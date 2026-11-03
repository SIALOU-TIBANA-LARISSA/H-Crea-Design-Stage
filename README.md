# H-Crea & Design

### Plateforme e-commerce de vente et de personnalisation de produits

## 1. Présentation du projet

**H-Crea & Design** est une plateforme e-commerce développée dans le cadre de mon stage professionnel chez H-Venture SARL.

Le projet vise à digitaliser l'activité commerciale de l'entreprise à travers une plateforme permettant aux clients de consulter un catalogue de produits, de personnaliser certaines créations, de gérer leur panier et de passer des commandes.

La plateforme intègre également un espace d'administration destiné à faciliter la gestion des produits, des catégories, des clients et des commandes.

Ce projet m'a permis de mettre en pratique mes compétences en analyse, conception, développement web, gestion de bases de données et déploiement d'applications.

---

## 2. Contexte et objectifs

L'objectif principal est de proposer une solution numérique permettant de :

* Présenter les produits de manière organisée.
* Faciliter la recherche et la consultation des produits.
* Permettre aux clients de personnaliser certaines créations.
* Simplifier le processus de commande.
* Centraliser la gestion des produits et des commandes.
* Faciliter le suivi de l'activité depuis un espace d'administration.
* Améliorer la communication avec les clients grâce à l'intégration d'un service SMS.

---

## 3. Analyse des besoins

La plateforme répond aux besoins de deux catégories principales d'utilisateurs.

### 3.1. Les clients

Les clients peuvent :

* Consulter le catalogue des produits.
* Parcourir les différentes catégories.
* Rechercher des produits.
* Créer un compte et se connecter.
* Ajouter des articles au panier.
* Gérer le contenu de leur panier.
* Personnaliser certains produits.
* Transmettre leurs propres fichiers de personnalisation.
* Consulter les aperçus des créations personnalisées.
* Effectuer une commande.
* Contacter l'entreprise via un formulaire de contact.

### 3.2. Les administrateurs

L'espace d'administration permet, selon les autorisations attribuées :

* De gérer les produits.
* De gérer les catégories.
* De consulter et gérer les clients.
* De gérer les utilisateurs administrateurs.
* De gérer les rôles et les permissions.
* De consulter et traiter les commandes.
* De gérer les annulations de commandes selon les droits accordés.

---

## 4. Conception du système

La phase de conception a permis de structurer le fonctionnement de la plateforme avant et pendant son développement.

Les travaux de conception du projet s'appuient sur les approches suivantes :

### 4.1. Analyse fonctionnelle

Identification des acteurs, des besoins et des principales fonctionnalités de la plateforme.

### 4.2. Modélisation UML

Utilisation de la modélisation UML pour représenter les interactions entre les utilisateurs et le système ainsi que l'organisation fonctionnelle de l'application.

### 4.3. Modélisation Merise

Utilisation de la méthode Merise pour structurer les données et préparer leur implémentation dans la base de données.

Les niveaux de modélisation concernés comprennent :

* MCD : Modèle Conceptuel de Données.
* MLD : Modèle Logique de Données.
* MPD : Modèle Physique de Données.

### 4.4. Organisation des processus

La modélisation des processus métier permet de représenter les différents enchaînements d'activités liés au fonctionnement de la plateforme.

---

## 5. Architecture technique

L'application repose sur une architecture web organisée autour de plusieurs composants.

### Frontend

La partie frontend assure l'affichage des pages et les interactions avec les utilisateurs.

Technologies utilisées :

* HTML5
* CSS3
* JavaScript
* Tailwind CSS
* Laravel Blade
* Vite

### Backend

Le backend assure le traitement des requêtes, l'application des règles métier, la gestion des utilisateurs et les opérations sur les données.

Technologies utilisées :

* PHP
* Laravel
* API REST
* Laravel Sanctum

### Base de données

La base de données relationnelle permet de stocker et d'organiser les informations nécessaires au fonctionnement de la plateforme.

* MySQL : environnement local et production.
* PostgreSQL : utilisé lors des premiers essais de déploiement sur Render.

---

## 6. Fonctionnalités développées

### 6.1. Catalogue et recherche

* Affichage des produits.
* Organisation par catégories.
* Recherche de produits.
* Consultation des détails des produits.

### 6.2. Personnalisation des produits

La plateforme permet la personnalisation de certaines créations à partir de fichiers numériques.

Formats pris en charge selon les produits :

* STL
* SVG
* DXF

Les clients peuvent notamment :

* Transmettre leurs propres fichiers SVG ou DXF.
* Choisir certaines options de rendu.
* Sélectionner des matériaux ou couleurs disponibles, notamment Bois, Plexiglass, Noir et Rouge.
* Visualiser un aperçu de leur création personnalisée.

Les fichiers déjà associés aux produits peuvent également être visualisés selon les formats disponibles.

### 6.3. Gestion des comptes

* Création de compte.
* Connexion et déconnexion.
* Authentification des utilisateurs.
* Gestion des accès selon les rôles et permissions.

### 6.4. Gestion du panier et des commandes

* Ajout de produits au panier.
* Consultation du panier.
* Modification du contenu du panier.
* Traitement des commandes.
* Gestion des commandes depuis l'administration.
* Gestion des annulations selon les autorisations.

### 6.5. Communication par SMS

Intégration d'une API SMS pour accompagner certaines opérations du parcours utilisateur, notamment l'inscription et les notifications.

### 6.6. Formulaire de contact

Mise à disposition d'un formulaire permettant aux visiteurs de transmettre leurs demandes à l'entreprise.

### 6.7. Administration

L'espace d'administration centralise les opérations de gestion :

* Gestion des produits et catégories.
* Gestion des clients.
* Gestion des administrateurs.
* Gestion des rôles et permissions.
* Gestion des commandes.

---

## 7. Base de données

La base de données permet de structurer les informations de la plateforme et de gérer les relations entre les différentes entités métier.

Elle prend notamment en charge les données relatives :

* Aux utilisateurs et aux clients.
* Aux administrateurs et à leurs autorisations.
* Aux produits.
* Aux catégories.
* Aux paniers et articles associés.
* Aux commandes.
* Aux données nécessaires à la personnalisation des produits.

La gestion et la consultation de la base de données ont notamment été réalisées avec les outils adaptés à l'environnement de développement, dont Beekeeper Studio et les outils MySQL.

---

## 8. Sécurité et authentification

Plusieurs mécanismes sont utilisés pour sécuriser l'application :

* Authentification des utilisateurs.
* Gestion des rôles et des permissions.
* Contrôle des accès aux fonctionnalités d'administration.
* Utilisation de Laravel Sanctum pour la gestion de l'authentification par API.
* Gestion des paramètres sensibles à travers les variables d'environnement.

Les informations confidentielles ne doivent pas être exposées dans le dépôt GitHub.

---

## 9. Tests et validation

Des vérifications ont été effectuées au cours du développement afin de contrôler le fonctionnement des différentes fonctionnalités.

Les principaux éléments vérifiés concernent :

* Les opérations d'inscription et de connexion.
* La gestion du catalogue.
* Les opérations sur le panier.
* Le traitement des commandes.
* Les fonctionnalités de personnalisation.
* Les interactions entre le frontend, le backend et la base de données.
* Le comportement de l'application après son déploiement.

---

## 10. Déploiement et mise en production

Le projet a connu plusieurs étapes de préparation et de déploiement.

### 10.1. Environnement de développement

Utilisation d'un environnement local pour développer l'application, configurer la base de données et vérifier les fonctionnalités.

### 10.2. Environnement de test

Utilisation de Render lors des premiers essais de déploiement, avec PostgreSQL comme système de gestion de base de données dans cet environnement.

### 10.3. Mise en production

Le site a finalement été déployé sur Hostinger avec une base de données MySQL.

Cette étape a nécessité la préparation de l'environnement d'hébergement, la configuration de l'application et la vérification de son fonctionnement en ligne.

---

## 11. Outils et environnement de travail

| Outil              | Utilisation                                          |
| ------------------ | ---------------------------------------------------- |
| Visual Studio Code | Développement et édition du code                     |
| Git                | Gestion des versions                                 |
| GitHub             | Hébergement et suivi du code source                  |
| Composer           | Gestion des dépendances PHP                          |
| NPM                | Gestion des dépendances frontend                     |
| MySQL              | Gestion de la base de données                        |
| Beekeeper Studio   | Consultation et administration de la base de données |
| phpMyAdmin         | Administration de MySQL                              |
| Docker             | Environnement de travail et essais techniques        |
| Render             | Premiers essais de déploiement                       |
| Hostinger          | Hébergement en production                            |
| FileZilla          | Transfert des fichiers vers l'hébergement            |

---

## 12. Installation en local

### Prérequis

* PHP compatible avec la version de Laravel utilisée.
* Composer.
* MySQL.
* Node.js et NPM.

### Installation

1. Cloner le dépôt :

```bash
git clone https://github.com/SIALOU-TIBANA-LARISSA/Mon-Nouveau-Projet-Electro.git
```

2. Accéder au dossier backend :

```bash
cd Mon-Nouveau-Projet-Electro/Backend
```

3. Installer les dépendances PHP :

```bash
composer install
```

4. Copier le fichier `.env.example` et créer un fichier `.env`.

5. Configurer les paramètres de connexion à la base de données MySQL dans le fichier `.env`.

6. Générer la clé de l'application :

```bash
php artisan key:generate
```

7. Exécuter les migrations si la configuration et les migrations sont prêtes :

```bash
php artisan migrate
```

8. Installer les dépendances frontend :

```bash
npm install
```

9. Compiler les ressources :

```bash
npm run build
```

10. Démarrer le serveur Laravel :

```bash
php artisan serve
```

---

## 13. Organisation du dépôt

```text
Mon-Nouveau-Projet-Electro/
│
├── README.md
│
└── Backend/
    ├── app/
    ├── bootstrap/
    ├── config/
    ├── database/
    ├── public/
    ├── resources/
    ├── routes/
    ├── storage/
    ├── tests/
    ├── artisan
    ├── composer.json
    ├── composer.lock
    └── README.md
```

Le README principal présente l'ensemble du projet. Le README situé dans `Backend/` apporte des informations complémentaires sur la partie backend.

---

## 14. Compétences mises en pratique

Ce projet m'a permis de mettre en pratique et de renforcer mes compétences dans plusieurs domaines :

* Analyse des besoins et compréhension fonctionnelle.
* Conception et modélisation de systèmes d'information.
* Développement backend avec PHP et Laravel.
* Développement d'interfaces web avec Blade, JavaScript et Tailwind CSS.
* Conception et exploitation de bases de données relationnelles.
* Intégration d'API.
* Authentification et gestion des autorisations.
* Gestion de versions avec Git et GitHub.
* Déploiement et configuration d'une application web.
* Résolution de problèmes techniques.

---

## 15. Contexte de réalisation

**Projet réalisé dans le cadre d'un stage école chez H-Venture SARL.**

Ce travail m'a permis de participer à la réalisation d'une solution e-commerce et de mettre en application les connaissances acquises durant ma formation en développement web et mobile.

**Technologies principales :** PHP, Laravel, MySQL, JavaScript, Tailwind CSS, Laravel Sanctum.

**Déploiement :** Hostinger.

**Auteur :** SIALOU TIBANA LARISSA
Développeuse d'applications et de sites web.

