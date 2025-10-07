# TechBlog

**TechBlog** est un blog communautaire développé avec **Symfony**, conçu pour publier des articles technologiques, les organiser par catégories, permettre les commentaires et gérer un espace membre sécurisé. Ce projet sert également d'apprentissage pour maîtriser les bonnes pratiques Symfony.

## Fonctionnalités

- Page d’accueil responsive avec Bootstrap 5  
- Gestion des articles et catégories (Actualités, Tutoriels, Tests, Opinion, Événements)  
- Inscription et connexion des utilisateurs (lecteurs, auteurs, administrateurs)  
- Création, modification et suppression d’articles  
- Système de commentaires sur les articles  
- Barre de recherche et pagination  
- Tableau de bord administrateur pour gérer le contenu  

## Installation

1. Cloner le dépôt :  
   ``bash
   git clone https://github.com/ton-utilisateur/techblog.git
   cd techblog
``

2. Installer les dépendances :

   ```bash
   composer install
   ```
3. Configurer la base de données dans `.env.local`
4. Créer la base et exécuter les migrations :

   ```bash
   php bin/console doctrine:database:create
   php bin/console doctrine:migrations:migrate
   php bin/console doctrine:fixtures:load
   ```
5. Lancer le serveur :

   ```bash
   symfony serve
   ```
6. Accéder à l’application : [http://localhost:8000](http://localhost:8000)

## Technologies

* Symfony 6.x
* PHP 8.x
* Doctrine ORM
* Twig
* Bootstrap 5
* SQLite (ou MySQL/MariaDB pour production)