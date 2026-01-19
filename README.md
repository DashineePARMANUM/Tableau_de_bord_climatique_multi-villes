# Tableau de bord climatique multi-villes
Projet en pair pour SDS 3786 - Laboratoire en science des données

---

## Fichiers et dossiers
- **`code`:**
  - **`Arielle`** = code ecrit par ma partenaire :
    - `IMPUTATION&CLUSTERING&TIME_SERIES_SDS3786_Groupe5.ipynb` = code pour les sections: imputation, clustering et series temporelles
  - **`Dashinee`** = code ecrit par moi :
    - `project_EDA_SDS3786_Groupe5.ipynb` = analyse exploratoire des données
    - `project_Multi_ville&Cartes_SDS3786_Groupe5.ipynb` = multi ville et cartes
    - `project_dashboard_SDS3786_Groupe5.ipynb` = dashboard
- **`data`** = jeux de données :
  - `ville_2.csv` = fichiers dont les colonnes ont été uniformisées directement dans Excel
  - `ville_4.csv` = fichiers dont les données relatives à la neige (Ottawa/Vancouver) et à la pression (autres) ont été supprimées afin de ne contenir que les colonnes présentes dans les 6 jeux de données
  - `ville_clean.csv` =  fichiers imputés
- **`docs`:**
  - `Étape1-Proposition_de_projet-SDS3786-Groupe5.pdf` = proposition initiale du project
  - `Étape2-Présentation_du_projet-SDS3786-Groupe5.pdf` = diapositifs pour la presentation en classe
  - `project_rapport_SDS3786_Groupe5.pdf` = rapport utilisé pour la presentation video finale

## Compétences démontrées
J'ai travaillé sur :
- Collecte des données = téléchargement et sélection de fichiers CSV
- Nettoyage et Fusion = uniformisation, format des dates, suppression de colonnes
- Analyse exploratoire (EDA) = statistiques descriptives et visualisations
- Multi-ville et cartes = comparaisons entre villes et cartes interactives
- Implémentation Python (Panel/HvPlot) = dashboard et visualisations interactives
- Tests et Ajustements = vérification de l’interactivité et cohérence globale
- Rapport final (en collaboration avec ma partenaire) =rédaction et synthèse des résultats

## Utilisation

## Source de données
- **Ottawa et Vancouver =** Les fichiers CSV ont été téléchargés pour les années 2020 à 2024 (un fichier par année) à partir des pages suivantes (données pour 2020) : [Ottawa](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2011-12-14%7C2025-03-15&dlyRange=2011-12-15%7C2025-03-14&mlyRange=%7C&StationID=49568&Prov=ON&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=14&searchMethod=contains&Month=1&Day=15&txtStationName=ottawa&timeframe=2&Year=2020) et [Vancouver](https://climate.weather.gc.ca/climate_data/daily_data_e.html?hlyRange=2013-06-11%7C2025-03-15&dlyRange=2013-06-13%7C2025-03-15&mlyRange=%7C&StationID=51442&Prov=BC&urlExtension=_e.html&searchType=stnName&optLimit=yearRange&StartYear=1840&EndYear=2025&selRowPerPage=25&Line=41&searchMethod=contains&txtStationName=vancouver&timeframe=2&Day=15&Year=2020&Month=1), puis combinés dans Excel afin d’obtenir une seule base de données complète couvrant la période 2020-2024 (Ottawa = OTTAWA INTL A, Vancouver = VANCOUVER INTL A).
- **Plaisance, Vacoas, Cotonou et Parakou =** Les fichiers CSV ont été téléchargés en choisisant la periode de 01/01/2020 - 12/31/2024 à partir des pages suivantes : [Plaisance](https://meteostat.net/en/station/61990?t=2020-01-01/2024-12-31&utm), [Vacoas](https://meteostat.net/en/place/mu/vacoas?s=61995&t=2026-01-05/2026-01-12), [Cotonou](https://meteostat.net/en/place/bj/cotonou?s=65344&t=2026-01-05/2026-01-12) et [Parakou](https://meteostat.net/en/place/bj/parakou?s=65330&t=2026-01-05/2026-01-12).

---
*Contact: dashinee.parmanum@gmail.com*  
*LinkedIn: https://www.linkedin.com/in/dashinee-parmanum/*
