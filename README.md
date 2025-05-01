📦 Student List – Mini-projet Docker
Ce projet est une preuve de concept (POC) visant à dockeriser une application web composée de deux modules (API + interface PHP) pour une entreprise fictive, POZOS.

🎯 Objectifs
Appliquer les bonnes pratiques Docker sur une application existante

Déployer une architecture découplée avec docker-compose

Gérer le cycle de vie des conteneurs, les volumes, les ports et l’authentification

Mettre en place un registry Docker privé

🧱 Stack technique
Docker / Docker Compose

Flask (API Python)

PHP / Apache (interface web)

CentOS 7.6 (VM)

Private Docker Registry

⚙️ Fonctionnement de l’application
L’API Flask fournit une liste d’élèves via un fichier JSON (authentification requise)

L’interface PHP consomme cette API et affiche les données côté client

Chaque composant tourne dans un conteneur dédié et communique via une infrastructure définie en docker-compose.yml.

🔧 Réalisations techniques
Création des Dockerfiles pour l’API

Configuration du docker-compose pour orchestrer les services

Gestion des volumes persistants et des réseaux personnalisés

Déploiement d’un Docker Registry privé avec interface web

Push de l’image construite dans le registry
