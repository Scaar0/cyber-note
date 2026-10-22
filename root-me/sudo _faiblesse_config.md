# sudo - faiblesse de configuration

Plateforme : Root-Me (catégorie App - Script)
Date : 21/10/2026
Difficulté : très facile
Durée : environ 30 min

## Objectif
Trouver le mot de passe écrit dans un fichier en exploitant les effets de bord des droits de certains fichiers.

## Ce que j'ai compris
- La vraie utilité de `sudo` est d'exécuter des commandes avec des droits différents des nôtres, pas seulement des actions root.
- Les nouveaux accès que nous offre `sudo` sont définis dans `/etc/sudoers`.
- Il faut donc faire attention aux droits que l'on donne aux groupes, y compris dans la configuration de `/etc/sudoers`.

## Commandes et outils utilisés
- `ls -al` : regarder les droits des fichiers, cachés ou non.
- `pwd` : pour savoir quel était mon répertoire actuel.
- `sudo -l` : afficher l'ensemble des commandes qu'on est autorisé à exécuter via sudo.
- `man sudo` : pour vérifier comment utiliser un autre utilisateur avec sudo.
- `sudo -u nom_utilisateur commande` : syntaxe pour exécuter une commande en tant qu'un utilisateur précis.

## Ce qui m'a bloqué
Je n'avais pas vu qu'on pouvait utiliser un autre utilisateur avec `sudo -u`. J'ai ensuite raté le nom exact de l'utilisateur, ce qui m'a coûté du temps.

## À retenir
Les modifications de `/etc/sudoers` doivent être extrêmement bien réfléchies : un `*` de trop et ça peut être le chaos. Il faut aussi toujours limiter au maximum les droits sur les fichiers et penser à les modifier, plutôt que de laisser les droits par défaut.