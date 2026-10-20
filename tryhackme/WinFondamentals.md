# Windows Fundamentals 1

Plateforme : TryHackMe (parcours : Windows Fundamentals 1)
Date : 19/10/2026
Difficulté : facile
Durée : 25min

## Objectif
Découvrir l'organisation d'un système Windows et ses outils de gestion des fichiers et d'administration de base.

## Notions clés
- Comment marche les fichiers Windows
- Comment marche les droits sur les fichiers/dossiers Windows
- Comment windows gère les interaction users/administrateur

## Outils et emplacements à connaître
| Outil ou dossier | À quoi ça sert |
|---|---|
| Gestionnaire des tâches | Voir les processus en cours, les stopper |
| Panneau de configuration | configurer toute sorte de choses |
| C:\Windows\System32 | contient les fichiers les plus important de l'OS toute modification doit-être bien maitrisée |
| lusrmgr.msc | sert a gérer les utilisateurs |

## Lien avec la cybersécurité
Utile pour connaître comment marche la machine d'une potentielle victime et savoir ce que va chercher un attaquant. Permet de savoir où regarder pour voir si des utilisateurs ont des droits non prévu ou tout acte non désiré.

## Comparaison avec Linux
les droits sont gérer par seulement 3 groupes et 3 possiblité 'r', 'w' et 'x' et pour le user, le groupe, et les others, donc il y a plus de différence sur Windows.

## Ce qui m'a bloqué
N/A

## À retenir
Il faut faire attention au droit sur windows.

## Pour aller plus loin
comment un attaquant pourrait tenter d'utiliser ces connaissance la pour avoir des actes malveillant.