# Scolarite IRIS

Un système de gestion scolaire pour l'établissement IRIS, permettant de gérer les classes, étudiants, professeurs, matières et utilisateurs.

## Description

Cette application web PHP permet de :
- Gérer les classes (ajout, modification, suppression, consultation)
- Gérer les étudiants (ajout, modification, suppression, consultation)
- Gérer les professeurs (ajout, modification, suppression, consultation)
- Gérer les matières (ajout, modification, suppression, consultation)
- Authentification des utilisateurs

L'application utilise une architecture MVC (Modèle-Vue-Contrôleur) et une base de données MySQL.

## Prérequis

- XAMPP (ou un serveur Apache avec PHP et MySQL)
- Navigateur web

## Installation

1. **Téléchargez et installez XAMPP** depuis [https://www.apachefriends.org/](https://www.apachefriends.org/)

2. **Démarrez XAMPP** :
   - Lancez le panneau de contrôle XAMPP
   - Démarrez les modules Apache et MySQL

3. **Placez le projet** :
   - Copiez le dossier du projet dans `C:\xampp\htdocs\Scolarite`

4. **Importez la base de données** :
   - Ouvrez phpMyAdmin (http://localhost/phpmyadmin)
   - Créez une nouvelle base de données nommée `scolarite_iris_2026_2a`
   - Importez le fichier `sql/scolarite_iris_2026_2A.sql`

5. **Accédez à l'application** :
   - Ouvrez votre navigateur
   - Allez à l'adresse : `http://localhost/Scolarite`

## Utilisation

1. **Connexion** :
   - Utilisez les identifiants par défaut :
     - Email : a@gmail.com
     - Mot de passe : 123

2. **Navigation** :
   - Cliquez sur les icônes pour accéder aux différentes sections :
     - Accueil
     - Classes
     - Étudiants
     - Professeurs
     - Matières
     - Déconnexion

3. **Gestion des données** :
   - Dans chaque section, vous pouvez ajouter, modifier, supprimer et consulter les enregistrements

## Structure du projet

```
Scolarite/
├── index.php                 # Point d'entrée de l'application
├── controleur/               # Contrôleurs
│   ├── controleur.class.php  # Classe contrôleur principale
│   ├── home.php              # Page d'accueil
│   ├── gestion_classes.php   # Gestion des classes
│   ├── gestion_etudiants.php # Gestion des étudiants
│   ├── gestion_profs.php     # Gestion des professeurs
│   ├── gestion_matieres.php  # Gestion des matières
│   └── erreur.php            # Page d'erreur
├── modele/                   # Modèles
│   └── modele.class.php      # Classe modèle
├── vue/                      # Vues
│   ├── vue_connexion.php     # Formulaire de connexion
│   ├── vue_insert_classe.php # Formulaire ajout classe
│   ├── vue_select_classes.php # Liste des classes
│   └── ...                   # Autres vues
├── sql/                      # Scripts SQL
│   └── scolarite_iris_2026_2A.sql # Base de données
└── images/                   # Images et icônes
```

## Technologies utilisées

- **PHP** : Langage de programmation côté serveur
- **MySQL** : Système de gestion de base de données
- **HTML/CSS** : Structure et style des pages web
- **JavaScript** : Interactivité côté client (si applicable)

## Dépannage

### Problèmes courants

1. **Erreur de connexion à la base de données** :
   - Vérifiez que MySQL est démarré dans XAMPP
   - Vérifiez les identifiants de connexion dans `modele/modele.class.php`

2. **Page blanche** :
   - Vérifiez les logs d'erreur PHP dans `C:\xampp\php\logs\php_error_log`
   - Assurez-vous que tous les fichiers sont présents

3. **Impossible d'accéder à phpMyAdmin** :
   - Vérifiez que Apache et MySQL sont démarrés
   - Essayez `http://localhost/phpmyadmin`

### Support

Pour toute question ou problème, contactez l'administrateur système.

## Licence

Ce projet est destiné à un usage éducatif.