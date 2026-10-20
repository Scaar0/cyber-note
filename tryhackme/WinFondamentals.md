# Windows Fundamentals

## Windows Fundamentals 1

Plateforme : TryHackMe (parcours : Windows Fundamentals 1)
Date : 19/10/2026
Difficulté : facile
Durée : 25 min

### Objectif
Découvrir l'organisation d'un système Windows et ses outils de gestion des fichiers et d'administration de base.

### Notions clés
- Comment fonctionnent les fichiers Windows
- Comment fonctionnent les droits sur les fichiers et dossiers Windows
- Comment Windows gère les interactions entre utilisateurs et administrateurs

### Outils et emplacements à connaître
| Outil ou dossier | À quoi ça sert |
|---|---|
| Gestionnaire des tâches | Voir les processus en cours et les arrêter |
| Panneau de configuration | Configurer de nombreux paramètres du système |
| C:\Windows\System32 | Contient les fichiers les plus importants du système, toute modification doit être bien maîtrisée |
| lusrmgr.msc | Gérer les utilisateurs |

### Lien avec la cybersécurité
Utile pour comprendre comment fonctionne la machine d'une victime potentielle et savoir ce que cherche un attaquant. Permet de savoir où regarder pour voir si des utilisateurs ont des droits non prévus ou tout acte non désiré.

### Comparaison avec Linux
Sous Linux, les droits sont gérés par seulement 3 classes (propriétaire, groupe, autres) et 3 permissions (r, w, x). Windows gère les droits de façon plus fine, ce qui laisse plus de possibilités.

### Ce qui m'a bloqué
N/A

### À retenir
Il faut faire attention aux droits sous Windows.

### Pour aller plus loin
Comment un attaquant pourrait-il utiliser ces connaissances à des fins malveillantes ?

---

## Windows Fundamentals 2

Plateforme : TryHackMe (parcours : Windows Fundamentals 2)
Date : 19/10/2026
Difficulté : facile
Durée : 15 min

### Objectif
Découvrir la configuration du système (msconfig) et les outils qu'elle offre.

### Notions clés
- Comment utiliser la configuration du système (System Configuration)
- A quoi servent les outils porposé dans msconfig: UAC, Registre, CMD etc...

### Outils et emplacements à connaître
| Outil | À quoi ça sert |
|---|---|
| Configuration du système (msconfig) | Donne accès à de nombreux outils de configuration de Windows |

### Commandes utilisées
- `winver.exe` : ouvre les informations sur la version de Windows
- `resmon.exe` : ouvre l'outil qui permet de visualiser les performances et l'usage des ressources de l'ordinateur local
- `UserAccountControlSettings.exe` : ouvre les paramètres de l'UAC
- `compmgmt.msc` : ouvre l'outil pour visualiser et configurer les paramètres du système et de ses composants
- `cmd.exe` : ouvre l'invite de commandes de Windows
- `regedt32.exe` : ouvre l'outil permettant de modifier le registre Windows

### Lien avec la cybersécurité
Sert à savoir où se trouvent les outils utiles et cruciaux pour des modifications importantes de la configuration de Windows. msconfig contrôle le démarrage, le Registre peut contrôler démarrage automatique et les stratégies/paramètres stratégiques Windows, la Gestion de l’ordinateur gère services/tâches planifiées et comptes, et UAC contrôle l’autorisation d’élévation. Pour un attaquant, c’est de la persistance et de l’escalade/privilèges ; pour un défenseur, c’est de l’audit, du durcissement et de la détection.

### Comparaison avec Linux
cmd.exe est l'équivalent du terminal Linux. Il y a de nombreuses commandes et cela permet d'utiliser Windows en ligne de commande (CLI).

### Ce qui m'a bloqué
N/A

### À retenir
System Configuration (msconfig) centralise de nombreux outils importants.

### Pour aller plus loin
Comment utiliser le registre en toute sécurité ?