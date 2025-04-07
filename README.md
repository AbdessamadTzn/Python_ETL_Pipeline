# Projet ETL en Python

## Description

Ce projet consiste à construire un pipeline ETL (Extract, Transform, Load) en Python, permettant d'extraire des données à partir de différentes sources (fichiers plats, API, base de données SQL Server locale), d'appliquer diverses transformations et contrôles de qualité, puis de charger les données prêtes à l'emploi dans un environnement cible.

## Objectifs

- Automatiser l'extraction des données depuis plusieurs sources
- Appliquer des vérifications de qualité de données (nulls, doublons, validation)
- Standardiser et transformer les données
- Préparer les données pour une exploitation fiable

## Sources de Données

- **Fichiers** : CSV
- **API** : RESTful APIs
- **Base de données** : SQL Server local

## Technologies

- **Python 3**
- **Pandas** : manipulation de données
- **Requests** : appel d'API
- **SQLAlchemy / pyodbc** : connexion SQL Server
- **dotenv** : gestion des variables d'environnement

## Pipeline ETL

### 1. Extraction

- Lecture de fichiers plats (CSV)
- Requêtes API
- Requêtes SQL pour extraire les données depuis la base locale

### 2. Transformation & Contrôles Qualité

- **Contrôle des valeurs nulles** : identification des colonnes critiques contenant des valeurs manquantes
- **Détection des doublons** : recherche de lignes identiques sur des colonnes clés
- **Validation de données** :
  - Format des dates
  - Plages de valeurs autorisées
  - Types de données (ex : entiers, float, chaînes)

### 3. Chargement

- Export vers un fichier intermédiaire nettoyé (CSV ou Parquet)
- Chargement dans une base de données cible ou un data warehouse (à définir)

....
