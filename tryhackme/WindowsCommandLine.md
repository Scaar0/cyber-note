# Windows Command Line

Plateforme : TryHackMe
Parcours ou catégorie : Windows Command Line
Date : 20/10/2026
Difficulté : facile
Durée : 30 min

## Objectif
Apprendre les commandes Windows essentielles.

## Notions clés
- Afficher les informations système basiques
- Vérifier et réparer la configuration réseau
- Gérer les fichiers et les dossiers
- Vérifier les processus en cours d'exécution

## Outils et commandes utilisés
| Outil ou commande | À quoi ça sert |
|---|---|
| `ipconfig` | Vérifier les informations du réseau |
| `ping target_name` | Vérifier qu'on peut accéder à un serveur cible |
| `nslookup example.com` | Cherche l'adresse IP d'un hôte ou d'un domaine et la renvoie |
| `netstat` | Affiche les connexions réseau actuelles et les ports utilisés |
| `cd` | Comme Linux |
| `dir` | Voir les dossiers enfants |
| `tree` | Représente visuellement les dossiers enfants |
| `mkdir` | Comme Linux |
| `type` | Comme `cat` |
| `copy fichier1 copie_fichier1` | Créer une copie du fichier |
| `move fichier destination` | Sert à déplacer un fichier à la destination voulue |
| `del` `erase` | Supprimer un fichier |
| `tasklist` | Affiche les processus en cours d'exécution |
| `tasklist /FI "imagename eq sshd.exe"` | Exemple d'utilisation pour afficher les processus dont l'Image Name est sshd.exe |
| `taskkill /PID target_pid` | Tuer le processus dont le PID est target_pid |
| `chkdsk` | Vérifie le système de fichiers et le stockage des disques pour détecter des erreurs ou des "bad sectors" |
| `driverquery` | Affiche la liste des drivers installés |
| `sfc /scannow` | Analyse les fichiers à la recherche de corruption et les répare si possible |
| `CommandeQuelconque /?` | `/?` permet d'afficher l'aide d'une commande |
| `shutdown /_` | Permet d'éteindre la machine (ou d'autres variantes) |

## Lien avec la cybersécurité
Permet d'interagir avec une machine sans interface graphique, ça demande moins de ressources et permet, si jamais la machine est bloquée graphiquement, de quand même y accéder. Un attaquant peut écrire un script batch ou PowerShell pour installer rapidement des malwares, etc., ou d'autres outils utiles pour lui. Un défenseur doit connaître ces commandes pour faire des diagnostics manuels de la machine et reconnaître un script batch ou PowerShell malveillant ou non.

## Comparaison avec Linux ou avec autre chose que je connais
Les commandes sont principalement différentes mais certaines reviennent, comme `cd` par exemple. La logique de fonctionnement principale reste la même, donc c'est facile de transférer ses connaissances.

## Ce qui m'a bloqué ou surpris
J'ai été surpris que la logique des commandes soit la même que celle de Linux, c'est un avantage.

## À retenir
Les commandes Windows doivent être maîtrisées pour intervenir rapidement sur une machine.

## Pour aller plus loin
Quelles sont les manipulations les plus courantes des attaquants avec cmd.exe ?