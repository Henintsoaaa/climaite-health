# Climate Risk and Health Prediction

Classification de décès selon leur sensibilité aux facteurs climatiques et environnementaux.

## Objectif

Prédire la variable `is_climate_sensitive` à partir de caractéristiques démographiques, géographiques, temporelles et climatiques.

## Données

- Âge, sexe et zone de résidence
- Date de décès
- Températures et précipitations
- Latitude, longitude et localisation
- Variables enrichies : altitude, NDVI, jours chauds, pluie, pente et températures agrégées

## Méthodes

- Analyse exploratoire et statistiques descriptives
- Nettoyage, imputation et encodage des variables
- Feature engineering temporel et environnemental
- Régression logistique comme baseline
- Validation croisée et analyse des performances
- Évaluation avec une métrique combinant F1-score et ROC-AUC

## Structure

- `climate_health_starter_notebook_.ipynb` : workflow principal
- `Train.csv` et `Test.csv` : données de compétition
- `climate_features.csv` : variables climatiques enrichies
- `*_submission.csv` : prédictions et variantes de soumission

La métrique officielle est `0.60 * F1 + 0.40 * ROC-AUC`.
