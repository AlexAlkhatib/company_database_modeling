# 🏢 Company Database Modeling

Modélisation complète d’une base de données d’entreprise avec **PowerDesigner**, incluant la conception conceptuelle/logique/physique et la génération automatique du script SQL MySQL.


## 📌 Objectif du projet

Ce projet consiste à **concevoir, modéliser et générer** une base de données professionnelle destinée à gérer les différentes entités d’une entreprise (employés, départements, projets, adresses…).
Le modèle final, réalisé sous **PowerDesigner**, permet de produire un **script SQL MySQL conforme**, normalisé, indexé et prêt à déployer.


## 📁 Contenu du dépôt

```
Company-Database-Modeling/
│
├── company_database_model.mpd     → Modèle PowerDesigner (PDM MySQL)
├── company_database.sql       → Script SQL généré (DDL complet)
├── ERD_Diagram.png            → Diagramme ER exporté
└── README.md
```


## 🧱 Modèle de données : entités principales

Le modèle couvre l’ensemble des besoins d’une entreprise :

* **Company** : informations générales de la société
* **Department** : départements internes
* **Employee** : employés, rôles, informations RH
* **Role** : fonctions/rôles salariés
* **Address** : adresses des bureaux (HQ, branches, etc.)
* **City** : villes référencées
* **Project** : projets de l’entreprise
* **EmployeeProject** : participation des employés aux projets
* **EmploymentHistory** : historique des affectations internes

Chaque table est liée par des **foreign keys**, correctement indexées, avec des stratégies de suppression cohérentes (`CASCADE`, `RESTRICT`, `SET NULL`).


## 🛠 Technologies & Outils

* **PowerDesigner** (modélisation LDM → PDM)
* **MySQL 8.x** (script DDL généré automatiquement)
* Modélisation relationnelle
* Normalisation (jusqu’à BCNF)
* Indexation et contraintes d’intégrité


## 🗂 Génération du script SQL

Le script MySQL final inclut :

* Création automatique de la base
* Définition des tables
* Clés primaires & étrangères
* Index simples et composites
* Contraintes (`UNIQUE`, `ENUM`, `NOT NULL`, `DEFAULT`)
* Relations avec `ON DELETE` / `ON UPDATE` adaptés
* Types MySQL optimisés (`BIGINT UNSIGNED`, `VARCHAR`, `DECIMAL`, `ENUM`…)

> 💡 Le script complet est disponible dans le dossier **sql/company_database.sql**.


## ▶️ Démonstration

Une démonstration de la **génération du script SQL depuis PowerDesigner** est présentée dans le guide du projet.

![http://url/to/img.gif](https://github.com/AlexAlkhatib/company_database_modeling/blob/main/Demo.gif)


## 👨‍💻 Auteur

**Alex Alkhatib**
Modélisation de bases de données · PowerDesigner · MySQL


## 📄 Licence

MIT License © 2025 Alex Alkhatib
