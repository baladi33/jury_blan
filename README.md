# 📊 Analyse de la Performance des Campagnes Marketing

## 📌 Contexte du projet

Ce projet de **Data Analysis** a pour objectif d’évaluer l’efficacité des campagnes marketing d’une entreprise et d’identifier les facteurs ayant un impact sur les ventes et le comportement des clients.

Le dataset contient des informations relatives à :

- 👤 Données démographiques des clients
- 📢 Campagnes marketing
- 🛍️ Produits achetés
- 🌐 Canaux d’achat (Web, Boutique, Catalogue)

L’analyse permet de transformer les données brutes en informations exploitables afin d’aider à la prise de décision stratégique.

---

# 🎯 Objectifs du Projet

Les principaux objectifs sont :

- Réaliser une **Analyse Exploratoire des Données (EDA)**
- Identifier les variables influençant les ventes
- Effectuer des **tests statistiques**
- Préparer et transformer les données avec **Power Query**
- Construire un **modèle de données Power BI**
- Créer un **dashboard interactif orienté business**

---

# 🛠️ Outils & Technologies

| Outil | Utilisation |
|---|---|
| Python | Analyse des données |
| pandas | Manipulation des données |
| numpy | Calcul numérique |
| matplotlib / seaborn | Visualisation |
| scipy | Tests statistiques |
| Power BI | Dashboard & Data Modeling |
| Power Query | Transformation des données |
| DAX | Mesures et KPIs |
| Excel | Analyse complémentaire |

---

# 📁 Structure du Projet

```bash
📦 Analyse-Performance-Campagnes-Marketing
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── eda_analysis.ipynb
│
├── powerbi/
│   └── Dashboard.pbix
│
├── images/
│   └── dashboard_screenshot.png
│
└── README.md
```

---

# 🔍 Étape 1 : Analyse Exploratoire des Données (EDA)

## ✅ Chargement des données

Les données sont chargées avec **pandas** afin d’effectuer une première exploration du dataset.

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
df.head()
```

---

## 📊 Analyses réalisées

### Variables numériques

- Revenus
- Dépenses
- Montant des achats

### Variables catégorielles

- Pays
- Campagnes marketing
- Produits
- Plateformes d’achat

---

## 📈 Visualisations

Les visualisations utilisées :

- Histogrammes → Distribution des ventes
- Boxplots → Détection des valeurs aberrantes
- Graphiques à barres → Analyse des campagnes

Exemple :

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.histplot(df["Sales"], kde=True)
plt.show()
```

---

## 🧹 Nettoyage des données

Les opérations de nettoyage comprennent :

- Gestion des valeurs manquantes
- Suppression des doublons
- Détection des anomalies
- Correction des types de données

---

# 📊 Étape 2 : Tests Statistiques

## ✅ Tests réalisés

### 🔹 t-test / ANOVA

Comparer les moyennes des ventes entre plusieurs groupes.

### 🔹 Test du Chi²

Étudier la relation entre deux variables catégorielles :

- Campagne acceptée vs Pays

### 🔹 Corrélation de Pearson

Mesurer la relation entre variables numériques.

---

## 📌 Interprétation

Les résultats permettent :

- D’identifier les variables significatives
- D’analyser les valeurs p
- De comprendre les facteurs influençant les ventes

---

# 🔄 Étape 3 : Transformation des Données (Power Query)

## ✅ Transformations réalisées

### Unpivot des colonnes

Transformation des données en format long pour :

- Campagnes
- Produits
- Plateformes

---

## 🧹 Nettoyage

- Renommage des colonnes
- Suppression des colonnes inutiles
- Gestion des types de données

---

## 🗂️ Structuration des tables

Création des tables suivantes :

- Clients
- Campagnes
- Produits
- Plateformes

---

# 🧩 Étape 4 : Modélisation des Données (Power BI)

## 🔗 Relations du modèle

- Clé principale : `ID_Client`
- Vérification des relations
- Contrôle de l’intégrité du modèle

---

## 📐 Mesures DAX

### Total des ventes

```DAX
Ventes Totales = SUM(Produits[Montant])
```

### Nombre de clients par campagne

```DAX
Clients Campagne = COUNT(Campagnes[ID_Client])
```

---

# 📈 Étape 5 : Tableau de Bord – Performance Marketing

## 📊 Visualisations du Dashboard

Le tableau de bord contient :

- 📢 Nombre de clients par campagne
- 💰 Chiffre d’affaires par campagne
- 📦 Répartition des ventes par produit
- 🛒 Répartition des achats par plateforme
- 🌍 Analyse par pays

---

## 🎛️ Interactivité

Des filtres dynamiques permettent d’analyser les données selon :

- Campagne
- Produit
- Pays
- Plateforme

---

# 💡 Insights Possibles

Grâce au dashboard, il est possible d’identifier :

- Les campagnes les plus performantes
- Les produits les plus vendus
- Les canaux d’achat les plus utilisés
- L’impact des caractéristiques clients sur les ventes

---

# 🚀 Résultats Attendus

À la fin du projet, le résultat attendu est :

✅ Un dashboard Power BI interactif  
✅ Des insights exploitables pour le business  
✅ Une meilleure compréhension du comportement client  
✅ Une aide à la prise de décision marketing  

---

# 📷 Aperçu du Dashboard

Ajouter ici une capture du tableau de bord :

```markdown
![Dashboard](images/dashboard_screenshot.png)
```

---

# ▶️ Lancer le Projet

## Installer les dépendances

```bash
pip install pandas numpy matplotlib seaborn scipy
```

## Exécuter le notebook

```bash
jupyter notebook
```

---

# 👨‍💻 Auteur
**Zoubair Baladi**  
Master en Systèmes & Télécommunications  
Passionné par la Data Analysis, Power BI et le Data Engineering.
