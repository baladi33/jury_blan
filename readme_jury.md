📊 Analyse de la Performance des Campagnes Marketing
📌 Contexte du projet

Dans le cadre d'un projet de Data Analysis, l'objectif est d'évaluer l'efficacité des campagnes marketing d'une entreprise et d'identifier les facteurs influençant les ventes.

Le dataset contient des informations sur :

Les clients (données démographiques)
Les campagnes marketing
Les produits achetés
Les canaux d'achat (Web, Boutique, Catalogue)
🎯 Objectifs
Réaliser une Analyse Exploratoire des Données (EDA)
Effectuer des tests statistiques pour mesurer l'impact des campagnes
Transformer et préparer les données avec Power Query
Construire un modèle de données dans Power BI
Créer un tableau de bord interactif orienté business
🛠️ Outils utilisés
Python : pandas, numpy, matplotlib, seaborn, scipy
Power BI : Power Query, DAX, Modélisation des données
Excel (facultatif)
📁 Structure du projet
📦 Analyse des performances de la campagne 
│ 
├── data/ 
│ └── dataset.csv 
│ 
├── notebooks/ 
│ └── eda_analysis.ipynb 
│ 
├── powerbi/ 
│ └── dashboard.pbix 
│ 
├── images/ 
│ └── dashboard_screenshot.png 
│ 
└── README.md
🔍 Étape 1 : Analyse Exploratoire des Données (EDA)
Chargement des données avec pandas
Identification des types de variables :
Les variables continuent (revenus, dépenses…)
Variables catégorielles (payes, campagnes…)
Analyses réalisées :
Statistiques descriptives :
Moyenne
Médiane
Min / Max
Type Écart
Visualisations :
Histogrammes (distribution des ventes)
Boxplots (détection des valeurs aberrantes)
Graphiques à barres (acceptation des campagnes)
Nettoyage des données :
Gestion des valeurs manquantes
Suppression des doublons
Détection des anomalies
📊 Étape 2 : Tests Statistiques
Tests utilisés :
t-test / ANOVA
→ Comparer les montants moyens des ventes entre groupes
Test du Chi²
→ Étudier la relation entre variables catégorielles
(ex : campagne acceptée vs pays)
Corrélation de Pearson
→ Mesurer la relation entre variables numériques
Interprétation :
Analyse des valeurs p
Identification des variables significatives influençant les ventes
🔄 Étape 3 : Transformation des Données (Power Query)
Transformation des données en format long (Unpivot) :
Campagnes
Produits
Plateformes
Nettoyage :
Renommage des colonnes
Suppression des colonnes inutiles
Structuration :
Création de tables :
Clients
Campagnes
Produits
Plateformes
🧩 Étape 4 : Modélisation des Données (Power BI)
Création des relations :
Clé principale : ID Client
Vérification :
Sens des filtres
Intégrité du modèle
Mesures DAX :
Total des ventes :
Ventes totales = SUM(Produits[Montant])
Nombre de clients par campagne :
Campagne de clients = COUNT(Campagnes[ID_Client])
📈 Étape 5 : Tableau de bord – Performance de la campagne
Visualisations :
📊 Nombre de clients par campagne
💰 Chiffre d'affaires par campagne et produit
📦 Répartition des ventes par produit (graphique à barres empilées)
🛒 Répartition des achats par plateforme
Interactivité :
Trancheurs :
Campagne
Produit
Pays
Filtres dynamiques
💡 Perspectives possibles
Identification des campagnes les plus performantes
Produits les plus vendus
Canaux d'achat
Impact des caractéristiques clients sur les ventes
🚀 Résultats attendus
Un tableau de bord clair et interactif
Des insights exploitables pour la prise de décision
Une meilleure compréhension du comportement client