# Bash - System 1

Plateforme : Root-Me (catégorie App - Script)
Date : 17/10/2026
Difficulté : facile
Durée : environ 30 min

## Objectif
Trouver comment lire un fichier protégé en exploitant un binaire SUID qui appelle une commande système sans préciser son chemin complet.

## Ce que j'ai compris
- Un binaire avec le bit SUID s'exécute avec les droits de son propriétaire (souvent root), et non avec les miens. S'il appelle une commande comme `ls` sans préciser son chemin complet, le système la cherche dans les dossiers listés par la variable PATH, dans l'ordre où ils y sont écrits.
- On peut modifier les variables comme PATH pour remplacer les commandes classiques par un programme malveillant à la place, et le script en C qui utilise system() exécute le code avec les droits dont on n'a pas forcément accès à l'origine.
- J'ai découvert qu'on pouvait écrire du shell dans un fichier pour l'exécuter ensuite, j'ai découvert la vulnérabilité des variables comme PATH.

## Commandes et outils utilisés
- `ls -al` : regarder les droits des fichiers cachés ou non.
- `pwd` : pour savoir quel était mon répertoire actuel.
- `nano [nom fichier]` : éditer un fichier dans le terminal directement.
- `man system` : system() permet d'exécuter des commandes dans le terminal en C.

## Ce qui m'a bloqué
Je n'avais pas compris qu'on pouvait réécrire la fonction `ls`, je ne connaissais pas le shell.
J'ai mis du temps à comprendre à quoi correspondait PATH.

## À retenir
Un binaire SUID qui appelle une commande système sans chemin complet est dangereux : n'importe qui peut détourner le PATH pour faire exécuter son propre code avec des droits élevés. Faire attention à ne pas laisser traîner des scripts et à sécuriser les scripts que j'ai sur mon ordinateur.