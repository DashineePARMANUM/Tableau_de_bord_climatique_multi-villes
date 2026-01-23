# Tableau de bord climatique multi-villes
Projet en binôme pour SDS 3786 - Laboratoire en science des données

## Fichiers et dossiers
- **`code`:**
  - **`Arielle`** = code écrit par ma partenaire :
    - `IMPUTATION&CLUSTERING&TIME_SERIES_SDS3786_Groupe5.ipynb` = code pour les sections: imputation, clustering et séries temporelles
  - **`Dashinee`** = code écrit par moi :
    - `project_EDA_SDS3786_Groupe5.ipynb` = analyse exploratoire des données
    - `project_Multi_ville&Cartes_SDS3786_Groupe5.ipynb` = multi-ville et cartes
    - `project_dashboard_SDS3786_Groupe5.ipynb` = dashboard
- **`data`** = jeux de données :
  - `ville_2.csv` = fichiers dont les colonnes ont été uniformisées directement dans Excel
  - `ville_4.csv` = fichiers dont les données relatives à la neige (Ottawa/Vancouver) et à la pression (autres) ont été supprimées afin de ne contenir que les colonnes présentes dans les 6 jeux de données
  - `ville_clean.csv` =  fichiers imputés
- **`docs`:**
  - `Étape1-Proposition_de_projet-SDS3786-Groupe5.pdf` = proposition initiale du project
  - `Étape2-Présentation_du_projet-SDS3786-Groupe5.pdf` = diapositifs pour la présentation en classe
  - `project_rapport_SDS3786_Groupe5.pdf` = rapport utilisé pour la présentation video finale

## Contributions
- Dashinee :
  - **Collecte des données**: Téléchargement des 6 fichiers CSV (Canada, Île Maurice, Bénin)
  - **Nettoyage et Fusion**: Uniformisation des colonnes, format de date, suppression des colonnes non utilisées
  - **Analyse exploratoire (EDA)**: Visualisation et calcul de statistiques descriptives pour toutes les villes
  - **Multi-ville et cartes**: Graphiques comparatifs, cartes avec couleurs/clusters, tooltips, indicateurs par ville
  - **Implémentation Python (Panel/HvPlot)**: Codage du tableau de bord et intégration des visualisations
  - **Tests et Ajustements**: Vérification de l’interactivité, cohérence générale et ajustements 
  - **Rapport final (travail collaboratif)**: Rédaction du PDF (résumé, captures d’écran, références)
- Arielle :
  - **Imputation** : Moyenne mobile / imputation saisonnière pour valeurs manquantes 
  - **Clustering** : Création de groupes climatiques (K-Means ou DBSCAN) pour toutes les villes
  - **Séries temporelles & prévisions** : Analyse des tendances 2020-2024 et prévisions pour les mois/année à venir
  - **Design du dashboard** : Choix des widgets, disposition, interactivité multi-villes
  - **Rapport final (travail collaboratif)**: Rédaction du PDF (résumé, captures d’écran, références)
  
## Utilisation
Pour ce projet, le développement a été réalisé dans un environnement Google Colab.  
Pour reproduire les résultats :
- Téléchargez le code et les jeux de données
- Importez les fichiers de données dans votre environnement Colab
- Exécutez les notebooks/scripts
  
## Source de données
- **Ottawa et Vancouver =** Les fichiers CSV ont été téléchargés pour les années 2020 à 2024 (un fichier par année) à partir des pages suivantes (données pour 2020) : [Ottawa](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2011-12-14%7C2025-03-15&dlyRange=2011-12-15%7C2025-03-14&mlyRange=%7C&StationID=49568&Prov=ON&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=14&searchMethod=contains&Month=1&Day=15&txtStationName=ottawa&timeframe=2&Year=2020) et [Vancouver](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2013-06-11%7C2025-03-15&dlyRange=2013-06-13%7C2025-03-15&mlyRange=%7C&StationID=51442&Prov=BC&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=41&searchMethod=contains&txtStationName=vancouver&timeframe=2&Day=15&Year=2020&Month=1), puis combinés dans Excel afin d’obtenir une seule base de données complète couvrant la période 2020-2024 (Ottawa = OTTAWA INTL A, Vancouver = VANCOUVER INTL A).
- **Plaisance, Vacoas, Cotonou et Parakou =** Les fichiers CSV ont été téléchargés en choisissant la période de 01/01/2020 - 12/31/2024 à partir des pages suivantes : [Plaisance](https://meteostat.net/en/station/61990?t=2020-01-01/2024-12-31&utm), [Vacoas](https://meteostat.net/en/place/mu/vacoas?s=61995&t=2026-01-05/2026-01-12), [Cotonou](https://meteostat.net/en/place/bj/cotonou?s=65344&t=2026-01-05/2026-01-12) et [Parakou](https://meteostat.net/en/place/bj/parakou?s=65330&t=2026-01-05/2026-01-12).

---
---
# Multi-city Climate Dashboard
Pair project for SDS 3786 - Data Science Laboratory (French section of SDS 3386)

## Files and Folders
- **`code`**
  - **`Arielle`** = code written by my partner  
    - `IMPUTATION_CLUSTERING_TIME_SERIES_SDS3786_Groupe5.ipynb` = code for the sections: imputation, clustering and time series
  - **`Dashinee`** = code written by me  
    - `project_EDA_SDS3786_Groupe5.ipynb` = exploratory data analysis  
    - `project_Multi_ville_Cartes_SDS3786_Groupe5.ipynb` = Multi-city analysis and maps  
    - `project_dashboard_SDS3786_Groupe5.ipynb` = dashboard  
- **`data`** = datasets
  - `ville_2.csv` = files whose columns were standardized directly in Excel
  - `ville_4.csv` = files with snow (Ottawa/Vancouver) and pressure (other cities) data removed to match columns across all 6 datasets
  - `ville_clean.csv` = imputed files
- **`docs`**
  - `Étape1_Proposition_de_projet_SDS3786_Groupe5.pdf` = initial project proposal  
  - `Étape2_Presentation_du_projet_SDS3786_Groupe5.pdf` = in-class presentation slides  
  - `project_rapport_SDS3786_Groupe5.pdf` = report used for final video presentation

## Contributions
- Dashinee :
  - **Collecte des données**: Téléchargement des 6 fichiers CSV (Canada, Île Maurice, Bénin)
  - **Nettoyage et Fusion**: Uniformisation des colonnes, format de date, suppression des colonnes non utilisé
  - **Analyse exploratoire (EDA)**: Visualisation et calcul de statistiques descriptives pour toutes les villes
  - **Multi-ville et cartes**: Graphiques comparatifs, cartes avec couleurs/clusters, tooltips, indicateurs par ville
  - **Implémentation Python (Panel/HvPlot)**: Codage du tableau de bord et intégration des visualisations
  - **Tests et Ajustements**: Vérification de l’interactivité, cohérence générale et ajustements 
  - **Rapport final (travail collaboratif)**: Rédaction du PDF (résumé, captures d’écran, références)
- Arielle :
  - **Imputation** : Moyenne mobile / imputation saisonnière pour valeurs manquantes 
  - **Clustering** : Création de groupes climatiques (K-Means ou DBSCAN) pour toutes les villes
  - **Séries temporelles & prévisions** : Analyse des tendances 2020-2024 et prévisions pour les mois/année à venir
  - **Design du dashboard** : Choix des widgets, disposition, interactivité multi-villes
  - **Rapport final (travail collaboratif)**: Rédaction du PDF (résumé, captures d’écran, références)

## Usage
This project was developed using Google Colab.  
To reproduce the results:
1. Download the code and datasets  
2. Upload the data files to your Colab environment  
3. Run the notebooks  

## Data Sources
- **Ottawa and Vancouver =** CSV files were downloaded for the years 2020 to 2024 (one file per year) from the following pages (data for 2020): [Ottawa](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2011-12-14%7C2025-03-15&dlyRange=2011-12-15%7C2025-03-14&mlyRange=%7C&StationID=49568&Prov=ON&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=14&searchMethod=contains&Month=1&Day=15&txtStationName=ottawa&timeframe=2&Year=2020) and [Vancouver](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2013-06-11%7C2025-03-15&dlyRange=2013-06-13%7C2025-03-15&mlyRange=%7C&StationID=51442&Prov=BC&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=41&searchMethod=contains&txtStationName=vancouver&timeframe=2&Day=15&Year=2020&Month=1), then combined in Excel to obtain a single complete database covering the period 2020-2024 (Ottawa = OTTAWA INTL A, Vancouver = VANCOUVER INTL A).
- **Plaisance, Vacoas, Cotonou and Parakou =** The CSV files were downloaded by selecting the period from 01/01/2020 to 12/31/2024 from the following pages : [Plaisance](https://meteostat.net/en/station/61990?t=2020-01-01/2024-12-31&utm), [Vacoas](https://meteostat.net/en/place/mu/vacoas?s=61995&t=2026-01-05/2026-01-12), [Cotonou](https://meteostat.net/en/place/bj/cotonou?s=65344&t=2026-01-05/2026-01-12) and [Parakou](https://meteostat.net/en/place/bj/parakou?s=65330&t=2026-01-05/2026-01-12).

---
---
*Honours Bachelor of Science in Statistics - University of Ottawa*  
*Contact: dashinee.parmanum@gmail.com*  
*LinkedIn: https://www.linkedin.com/in/dashinee-parmanum/*
