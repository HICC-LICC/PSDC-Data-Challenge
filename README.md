# Public Service Data Challenge HICC project

# README for Data Challenge Notebook

## Overview
Currently, shelters lack a centralized system for real-time bed availability tracking, leading to resource allocation challenges. This project aims to implement data analytics and predictive forecasting to enhance inventory management, usage analysis, and decision-making.  

By integrating these capabilities, shelters can optimize resource distribution, strengthening the support network for vulnerable populations. Housing Infrastructure and Communities Canada (HICC) aims to lead in Artificial Intelligence (AI) innovation, leveraging public shelter, census, and weather to build a predictive model on bed availability, which aligns with HICC’s goal of responsible AI use in social impact areas like housing. 

This initiative develops machine learning models using Alberta and Toronto shelter data, aligned with HICC’s framework for responsible Artificial Intelligence (AI). Models such as Random Forest, XGB Regressor, and Nearest Neighbor Analysis, used to build the model, are designed to respect ethical guidelines, supporting transparent and accountable AI deployment.

Predictive AI models forecast shelter space needs using interpretable models like Random Forest and XGB Regressor, adhering to HICC’s principles of transparency, accountability, and explainability. These models are scoped to improve operational efficiency and ensure consistent, accurate outcomes within the ethical boundaries of the framework.

**Important Note:** The dataset and code in this notebook are sourced from a clone of the Data Science Challenge repository hosted on DevOps. this work was conducted for the 2023-2024 Public Service Data Challenge: https://canada.governmentdatachallenge.com/. Users must update the repository clone to their own DevOps or Git environment for the notebook to function as expected. See the [Data Sources](#data-sources) section for more details.

## Table of Contents
1. [Requirements](#requirements)
2. [Data Sources](#data-sources)
3. [Notebook Structure](#notebook-structure)
4. [Key Features](#key-features)
5. [How to Use](#how-to-use)
6. [Outputs](#outputs)
7. [Future Enhancements](#future-enhancements)

---

## Requirements
To execute this notebook successfully, ensure you have the following installed:

- **Python 3.7+**
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

Install the libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Data Sources
This notebook processes data sourced from a cloned Data Science Challenge repository hosted on DevOps. To use this notebook:
1. Clone the original repository to your DevOps account or a personal Git environment.
2. Update the file paths in the notebook to reflect your repository's structure.

Example of cloning the repository:
```bash
git clone https://dev.azure.com/your-org/your-repo/_git/data-science-challenge
```

Ensure you modify the notebook's data loading paths to match your repository's folder structure.

---

## Notebook Structure
The notebook is organized into the following sections:

### 1. **Setup and Initialization**
- Importing necessary libraries.
- Setting global configurations for plots and warnings.

### 2. **Data Loading**
- Loading datasets from the cloned repository into pandas DataFrames.
- Inspecting the initial structure of the data (e.g., `.head()`, `.info()`).

### 3. **Data Cleaning**
- Handling missing values (e.g., filling, dropping).
- Removing duplicates.
- Ensuring consistent data types across columns.

### 4. **Feature Engineering**
- Creating new features based on domain knowledge.
- Encoding categorical variables.
- Normalizing or scaling numerical features.

### 5. **Exploratory Data Analysis (EDA)**
- Generating descriptive statistics.
- Visualizing data distributions and relationships using:
  - Histograms.
  - Box plots.
  - Correlation heatmaps.

### 6. **Modeling and Predictions**
- Splitting data into training and testing subsets.
- Applying machine learning algorithms such as linear regression or classification models.
- Evaluating model performance using metrics like accuracy, precision, recall, etc.

### 7. **Visualization**
- Creating plots to communicate key insights.
- Highlighting patterns and trends in the dataset.

---

## Key Features
1. **Data Cleaning**
   - Comprehensive handling of missing values and outliers.
2. **Feature Engineering**
   - Deriving insightful features for improved model performance.
3. **EDA**
   - Thorough analysis to uncover hidden patterns.
4. **Machine Learning Models**
   - Implementation of predictive models.
5. **Custom Visualizations**
   - Clear and concise charts to support analysis.

---

## How to Use
1. Clone the repository to your own DevOps or Git environment:
   ```bash
   git clone https://dev.azure.com/your-org/your-repo/_git/data-science-challenge
   ```
2. Modify the notebook's file paths to match your cloned repository's structure.
3. Open the notebook in Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook data_challenge_edit_cleaned.ipynb
   ```
4. Run the cells sequentially to reproduce the results.
5. Modify parameters or add custom code as needed.

---

## Outputs
- **Cleaned Dataset**: The processed dataset is ready for further analysis or modeling.
- **Visualization Charts**: Saved as PNG files (if applicable).
- **Model Predictions**: Output stored in a CSV file or displayed in the notebook.

---

## Future Enhancements
- Integration with larger datasets for scalability.
- Deployment of models as APIs for real-time predictions.
- Advanced feature selection techniques for improved accuracy.
- Automation of the entire data pipeline.

---

This README provides a detailed understanding of the notebook, ensuring ease of use and clarity for collaborators or future reference.

# Défi des données du service public Projet LICC

# README pour le cahier de défis de données

## Aperçu
Présentement, les refuges ne disposent pas d'un système centralisé de suivi en temps réel de la disponibilité des lits, ce qui pose des problèmes d'allocation des ressources. Ce projet vise à mettre en œuvre l'analyse des données et les prévisions afin d'améliorer la gestion des stocks, l'analyse de l'utilisation et la prise de décision.

En intégrant ces capacités, les refuges peuvent optimiser la distribution des ressources, renforçant ainsi le réseau de soutien aux populations vulnérables. Logement, Infrastructure et Collectivités Canada (LICC) vise à être le chef de file de l'innovation en matière d'intelligence artificielle (IA), en s'appuyant sur les refuges publics, le recensement et les conditions météorologiques pour construire un modèle prédictif de la disponibilité des lits, ce qui correspond à l'objectif de LICC d'utiliser l'IA de manière responsable dans des domaines à impact social tels que le logement.

Cette initiative développe des modèles d'apprentissage automatique en utilisant les données des refuges de l'Alberta et de Toronto, en accord avec le cadre du LICC pour une intelligence artificielle (IA) responsable. Des modèles tels que Random Forest, XGB Regressor et Nearest Neighbor Analysis, utilisés pour construire le modèle, sont conçus pour respecter les directives éthiques, soutenant un déploiement transparent et responsable de l'IA.

Les modèles d'IA prédictive prévoient les besoins en espaces d'hébergement à l'aide de modèles interprétables tels que Random Forest et XGB Regressor, en adhérant aux principes de transparence, de responsabilité et d'explicabilité du LICC. Ces modèles sont conçus pour améliorer l'efficacité opérationnelle et garantir des résultats cohérents et précis dans les limites éthiques du cadre.

**Note importante:** Le jeu de données et le code de ce carnet proviennent d'un clone du dépôt du défi de la science des données hébergé sur DevOps. Ce travail a été réalisé dans le cadre du défi de la science des données de la fonction publique 2023-2024 : https://canada.governmentdatachallenge.com/fr/. Les utilisateurs doivent mettre à jour le clone du dépôt dans leur propre environnement DevOps ou Git pour que le carnet fonctionne comme prévu. Voir la section [Sources de données](# Sources-de-données) pour plus de détails.

## Table des matières
1. [Exigences](#exigences)
2. [Sources de données](#sourcesdedonnées)
3. [Structure du carnet de notes](#structure-du-carnet-de-notes)
4. [Caractéristiques principales](#caractéristiques-clé)
5. [Mode d'emploi](#moded'emploi)
6. [Sorties](#sorties)
7. [Améliorations futures](#future-enhancements)

---

## Exigences
Pour exécuter ce cahier avec succès, assurez-vous que les éléments suivants sont installés :

- **Python 3.7+**
- Bibliothèques:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

Installez les bibliothèques à l'aide de pip :
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Sources de données
Ce bloc-notes traite des données provenant d'un référentiel cloné du Data Science Challenge hébergé sur DevOps. Pour utiliser ce carnet :
1. Clonez le dépôt original sur votre compte DevOps ou sur un environnement Git personnel.
2. Mettez à jour les chemins d'accès aux fichiers dans le carnet de notes pour refléter la structure de votre référentiel.

Exemple de clonage du dépôt:
```bash
git clone https://dev.azure.com/your-org/your-repo/_git/data-science-challenge
```

Assurez-vous de modifier les chemins de chargement des données du carnet pour qu'ils correspondent à la structure des dossiers de votre référentiel.

---

## Structure du carnet
Le carnet de notes est organisé selon les sections suivantes :

### 1. **Configuration et initialisation**
- Importation des bibliothèques nécessaires.
- Définition des configurations globales pour les tracés et les avertissements.

### 2. **Chargement des données**
- Chargement des ensembles de données du référentiel cloné dans les DataFrames pandas.
- Inspection de la structure initiale des données (par exemple, `.head()`, `.info()`).

### 3. **Nettoyage des données**
- Traitement des valeurs manquantes (par exemple, remplissage, abandon).
- Suppression des doublons.
- Assurer la cohérence des types de données entre les colonnes.

### 4. **Ingénierie des fonctionnalités**
- Création de nouvelles caractéristiques basées sur la connaissance du domaine.
- Encodage de variables catégorielles.
- Normalisation ou mise à l'échelle des caractéristiques numériques.
### 5. **Analyse exploratoire des données (AED)**
- Générer des statistiques descriptives.
- Visualisation des distributions de données et des relations à l'aide de :
  - Histogrammes.
  - Diagrammes en boîte.
  - Cartes thermiques de corrélation.

### 6. **Modélisation et prédictions**
- Diviser les données en sous-ensembles de formation et de test.
- Appliquer des algorithmes d'apprentissage automatique tels que des modèles de régression linéaire ou de classification.
- Évaluer les performances du modèle à l'aide de mesures telles que l'exactitude, la précision, le rappel, etc.

### 7. **Visualisation**
- Créer des graphiques pour communiquer des informations clés.
- Mettre en évidence les schémas et les tendances dans l'ensemble des données.

---

## Caractéristiques essentielles
1. **Nettoyage des données
   - Traitement complet des valeurs manquantes et des valeurs aberrantes.
2. **Ingénierie des caractéristiques**
   - Dérivation de caractéristiques pertinentes pour améliorer les performances du modèle.
3. **EDA**
   - Analyse approfondie pour découvrir des modèles cachés.
4. **Modèles d'apprentissage automatique**
   - Mise en œuvre de modèles prédictifs.
5. **Visualisations personnalisées
   - Graphiques clairs et concis pour soutenir l'analyse.

---

## Comment l'utiliser
1. Clonez le dépôt dans votre propre environnement DevOps ou Git :
   ```bash
   git clone https://dev.azure.com/your-org/your-repo/_git/data-science-challenge
   ```
2. Modifiez les chemins des fichiers du carnet pour qu'ils correspondent à la structure de votre référentiel cloné.
3. Ouvrez le notebook dans Jupyter Notebook ou JupyterLab :
   ``bash
   jupyter notebook data_challenge_edit_cleaned.ipynb
   ```
4. Exécutez les cellules séquentiellement pour reproduire les résultats.
5. Modifiez les paramètres ou ajoutez du code personnalisé si nécessaire.

---

## Extrants
- **Ensemble de données nettoyé** : L'ensemble de données traitées est prêt pour une analyse ou une modélisation plus poussée.
- Graphiques de visualisation** : enregistrés sous forme de fichiers PNG (le cas échéant).
- Prédictions du modèle** : Sortie stockée dans un fichier CSV ou affichée dans le carnet de notes.
---
## Améliorations futures
- Intégration d'ensembles de données plus importants pour une meilleure évolutivité.
- Déploiement de modèles en tant qu'API pour des prédictions en temps réel.
- Techniques avancées de sélection des caractéristiques pour une meilleure précision.
- Automatisation de l'ensemble du pipeline de données.
---
Ce README fournit une compréhension détaillée du notebook, assurant la facilité d'utilisation et la clarté pour les collaborateurs ou les références futures.
