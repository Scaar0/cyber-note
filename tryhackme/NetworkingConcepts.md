# Networking Concepts

Plateforme : TryHackMe
Parcours ou catégorie : Networking Concepts
Date : 22/10/2026
Difficulté : facile
Durée : 30 min

## Objectif
Découvrir le modèle OSI de l'ISO et la suite de protocoles TCP/IP.

## Notions clés
- Le modèle ISO OSI comporte 7 couches : 1 physique, 2 liaison de données, 3 réseau, 4 transport, 5 session, 6 présentation, 7 application.
- Adresses IP : il y a les publiques et les privées, de 0.0.0.0 à 255.255.255.255 en IPv4. Elles identifient la machine sur un réseau.
- TCP et UDP sont des protocoles de transport. UDP n'a pas de confirmation d'envoi, il est plus rapide que TCP. TCP s'assure que les données sont bien transmises avec un échange en 3 étapes. Ils fonctionnent avec les ports 1 à 65535.
- Telnet permet de se connecter à un autre système, de communiquer avec lui et d'exécuter des commandes textuelles. Il envoie tout en clair.

## Outils et commandes utilisés
| Outil ou commande | À quoi ça sert |
|---|---|
| Telnet | Permet de parler à différents serveurs en utilisant TCP |

## Lien avec la cybersécurité
Permet de comprendre comment fonctionnent les bases du réseau. Une meilleure compréhension facilite l'appréhension de problèmes ou de concepts plus compliqués plus tard. Par exemple, connaître les ports et les protocoles aide à interpréter les résultats d'un scan Nmap. Telnet envoie tout en clair, contrairement à SSH : l'utiliser est déjà une erreur.

## À retenir
Internet n'est pas magique, il a un fonctionnement précis qu'il faut connaître.

## Pour aller plus loin
Comment un attaquant et un défenseur utilisent-ils ces connaissances (couches, ports, protocoles) ?