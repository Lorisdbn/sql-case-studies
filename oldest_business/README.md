# World’s Oldest Businesses Analysis Project

![Aperçu](image.jpeg)

## Overview
Ce projet analyse les entreprises les plus anciennes encore en activité à travers le monde, tel que compilé par BusinessFinancing.co.uk. L’objectif est de comprendre la longévité des entreprises selon les pays, les catégories et les périodes historiques.

## Objectifs
1. Identifier le nombre total d’entreprises dans la base.  
2. Déterminer l’entreprise la plus ancienne (année de fondation minimale).  
3. Analyser la répartition des entreprises anciennes par continent.  
4. Comparer la création de nouvelles entreprises (depuis 1900) avec la base historique.

## Structure du dépôt / Data schema

### Tables `businesses` et `new_businesses`

| Column          | Description                                  | Data Type |
|-----------------|----------------------------------------------|-----------|
| `business`      | Name of the business                         | varchar   |
| `year_founded`  | Year the business was founded                | int       |
| `category_code` | Code for the business category               | varchar   |
| `country_code`  | ISO 3166-1 three-letter country code         | char      |

### Table `countries`

| Column          | Description                                              | Data Type |
|-----------------|----------------------------------------------------------|-----------|
| `country_code`  | ISO 3166-1 three-letter country code                     | varchar   |
| `country`       | Name of the country                                      | varchar   |
| `continent`     | Name of the continent the country exists in              | varchar   |

### Table `categories`

| Column           | Description                            | Data Type |
|------------------|----------------------------------------|-----------|
| `category_code`  | Code for the business category         | varchar   |
| `category`       | Description of the business category   | varchar   |
