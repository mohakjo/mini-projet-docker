# Mini-projet Docker – Student List App

Ce projet consiste à **dockeriser une application web composée de deux modules** (API Flask + Front PHP) pour une entreprise fictive, POZOS.

## Stack technique

- Docker
- Docker Compose
- Flask (API REST)
- PHP / Apache (interface utilisateur)
- CentOS (VM recommandée)

## 📂 Fichiers du projet

- `Dockerfile` : pour construire l’image de l’API Flask
- `docker-compose.yml` : pour orchestrer le déploiement de l’API et du front PHP
- `requirements.txt` : dépendances Python
- `student_age.json` : fichier JSON des étudiants
- `student_age.py` : script Python de l’API
- `index.php` : interface front
- `/website/` : dossier monté avec les fichiers PHP

## 🔧 Fonctionnalités

- L’**API Flask** fournit une liste d’élèves au format JSON
- Le **site PHP** consomme l’API et affiche les résultats
- Utilisation de **volumes**, **ports exposés**, **variables d’environnement**
- **Déploiement orchestré via Docker Compose**

## ▶️ Lancement

1. Construire l’image API :

```bash
docker build -t student-api .
```

## 

2. Lancer toute l’infrastructure :
```bash
docker-compose up -d
```

3. Accéder au front via le port défini et tester l’API avec curl :

```bash
curl -u toto:python http://localhost:5000/pozos/api/v1.0/get_student_ages
```

# 🎯 Objectifs pédagogiques
Appliquer les bonnes pratiques Docker

Utiliser Docker Compose pour structurer une application multi-conteneurs

Gérer des volumes, ports, réseaux et services

Comprendre l’architecture découplée


