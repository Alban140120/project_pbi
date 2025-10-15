## Description
Ce projet consiste à créer un reporting interactif sur Power BI avec versioning du projet au format .pbip. Il combine des données CSV sur les véhicules électriques avec des visualisations avancées, notamment l’intégration de Python pour certains visuels analytiques (ex. ACP).

Structure du modèle de données

Le modèle suit un schéma en étoile (Star Schema) :

DIM_BODY_TYPE – Types de carrosserie

DIM_BRAND – Marques de véhicules

DIM_DRIVE_TRAIN – Type de motorisation (électrique, hybride, etc.)

DIM_MODEL – Modèles de véhicules

FACT_TABLE – Table des mesures et indicateurs (KPI)

Des mesures ont été créées pour les visualisations Power BI (ex. vitesse, puissance, capacité de traction…).

## Visualisations par page

Page Brand / KPI

Filtre pour choisir le KPI étudié

Top 5 modèles pour le KPI sélectionné

Affichage du groupe de la marque (Stellantis, Ford, etc.) et du drapeau du pays

Page ACP (Analyse en Composantes Principales)

Visualisation multivariée des modèles en fonction des KPI

Possibilité de regrouper plusieurs modèles selon leurs caractéristiques

Page Carte

Carte interactive avec choix du KPI via filtre

Couleur sur la carte en fonction de l’importance du KPI

Indication du pays avec le KPI le plus faible et le plus élevé

Page Scatter / Tendances

Nuage de points pour étudier les tendances entre deux KPI

Choix d’une marque et de deux KPI à comparer (ex. vitesse max vs couple moyen)

Affichage de la droite de tendance

Page Summary

Matrice croisant pays et marque/modèle pour le KPI sélectionné

Top 5 et Flop 5 par marque

Feature Engineering

Création de nouvelles variables :

Pays d’origine de la marque

Nom du groupe de la marque

Logo de la marque au format PNG pour intégration dans les visuels

## Technologies et outils

Power BI Desktop pour le reporting interactif

Python pour l’ACP et certains visuels avancés

Git pour le versioning du projet (format .pbip)

CSV comme source de données initiale