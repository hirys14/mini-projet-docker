# mini-projet-docker

Ce projet a été réalisé dans le cadre de mon parcous Devops au BootCamp n°22 de EAZYTraining.

## Contexte

PayMyBuddy est une application de gestion des transactions financières entre amis. L'infrastructure actuelle est étroitement couplée et déployée manuellement, ce qui entraîne des inefficacités. Nous visons à améliorer l'évolutivité et à rationaliser le processus de déploiement à l'aide de Docker et de l'orchestration de conteneurs.

## Objectifs

- Amélioration des processus de déploiement
- Versionnage des versions d'infrastructure
- Mise en œuvre des meilleures pratiques pour Docker
- Utilisation de l'infrastructure en tant que code

## Infrastructure

L'infrastructure fonctionnera sur un serveur compatible Docker avec Ubuntu 20.04. Cette preuve de concept (POC) comprend la conteneurisation du backend Spring Boot et de la base de données MySQL et l'automatisation du déploiement à l'aide de Docker Compose.

### Composants :
-Backend (Spring Boot) : gère les données et les transactions des utilisateurs
-Base de données (MySQL) : stocke les utilisateurs, les transactions et les détails des comptes
-Orchestration : utilise Docker Compose pour gérer l'ensemble de la pile d'applications

## Application

PayMyBuddy est divisé en deux services principaux :

-Service backend (Spring Boot) :

Expose une API pour gérer les transactions et les interactions des utilisateurs
Se connecte à une base de données MySQL pour un stockage persistant

-Service de base de données (MySQL) :

Stocke les données utilisateur et transactionnelles
Exposé sur le port 3306 pour que le backend se connecte

## Travail à Faire

Mon travail consiste à :

- 1 - Provisionner une VM avec Ubuntu 20.04 comme OS
- 2 - Installer Docker , git et Docker-compose sur la VM
- 3 - Produire les Dockerfiles 
- 4 - Builder & Tester les images (Créer des conteneurs et les faire interagir les uns avec les autres) 
- 5 - Produire le docker-compose (**IAC**)
- 6 - Fournir un registre privé pour stocker les images


### Étapes 1 & 2 (*Provisionner une VM avec Centos7.6 comme OS*)

Pour provisionner la VM j'ai opté pour **Proxmox Ve** pour le deploiement de la VM et l'installation de **Docker, git et docker-compose**

la VM

<img src="/images/Capture1.JPG" alt="ma vm version">




