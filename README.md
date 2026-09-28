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

- `data/raw/` : données Train/Test et variables climatiques enrichies
- `notebooks/` : workflow d'analyse et de modélisation
- `submissions/` : prédictions et variantes de soumission
- `submissions/templates/` : format officiel de soumission
- `docs/` : dictionnaires de données

## Exécution

Depuis la racine du dépôt, ouvrir `notebooks/01_climate_health_baseline.ipynb` dans Jupyter.

Le notebook charge automatiquement les fichiers depuis `../data/raw/` et sauvegarde la soumission dans `../submissions/`.

La métrique officielle est `0.60 * F1 + 0.40 * ROC-AUC`.
