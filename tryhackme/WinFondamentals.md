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

Plateforme : TryHackMe (parcours : [nom du parcours])
Date : jj/mm/aaaa
Difficulté : facile
Durée : [environ X min]

### Objectif
[Une phrase : ce que la salle t'apprend.]

### Notions clés
- [Notion 1, avec tes mots]
- [Notion 2]
- [Notion 3]

### Outils et emplacements à connaître
| Outil | À quoi ça sert | Ce que j'y ai trouvé ou testé |
|---|---|---|
| [Configuration du système (msconfig)] | [...] | [...] |
| [Contrôle de compte utilisateur (UAC)] | [...] | [...] |
| [Gestion de l'ordinateur] | [...] | [...] |
| [Informations système (msinfo32)] | [...] | [...] |
| [Moniteur de ressources] | [...] | [...] |
| [Invite de commandes] | [...] | [...] |
| [Éditeur du Registre (regedit)] | [...] | [...] |

### Commandes utilisées
- `[commande]` : [ce qu'elle fait]
- `[commande]` : [ce qu'elle fait]

### Le Registre en une phrase
[Explique avec tes mots ce qu'est le Registre Windows et à quoi sert chacune de ses grandes ruches que tu as vues.]

### Lien avec la cybersécurité
[Pourquoi ces outils comptent. Par exemple : où un programme malveillant peut se cacher pour démarrer avec la machine, où regarder les journaux d'événements, comment repérer un processus suspect.]

### Comparaison avec Linux
[Équivalents que tu connais : services, cron, journaux dans /var/log, terminal, fichiers de configuration. Quelle est la différence principale avec le Registre ?]

### Ce qui m'a bloqué ou surpris
[Une ou deux lignes.]

### À retenir
[Une phrase de conclusion.]

### Pour aller plus loin
[Une question que tu te poses encore.]