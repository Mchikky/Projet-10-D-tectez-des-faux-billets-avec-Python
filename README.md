# Project 10: Detect counterfeit banknotes with Python 

## Objectives 
Detect counterfeit banknotes with Python by setting up a model capable of automatically identifying real and fake notes.
1. Implement models that would be able to automatically identify real from counterfeit banknotes, based solely on certain dimensions of the banknote and the elements that compose it.
2. Compare the models stating the significances.

## Data Preprocessing
1. Import billet.csv file
   
<img width="1187" alt="a" src="https://github.com/user-attachments/assets/5c956f3f-2a09-47fd-b081-398205ae4a6b" />

2. Studied the data values, checked for missing values and duplicates.
   
<img width="1040" alt="aa" src="https://github.com/user-attachments/assets/23e595b6-10ec-4758-92f0-221706c4beb1" />

3. Identified outliers
   
<img width="959" alt="aaa" src="https://github.com/user-attachments/assets/e47bbb28-d062-47ba-82ff-065c1a87e949" />


## Exploratory Data Analysis (EDA)
Conduct an exploratory and descriptive data analysis
1. Checked the distribution of the data

<img width="947" alt="aaa" src="https://github.com/user-attachments/assets/6a21cf1b-14ed-409e-8124-f89b72576961" />

2. Correlation

<img width="867" alt="aa" src="https://github.com/user-attachments/assets/3ceae67f-87c0-4c5f-9ae7-30533d791d88" />


3. Used linear regression to impute missing values.

<img width="973" alt="aaaa" src="https://github.com/user-attachments/assets/dc4881da-9782-47a8-baa1-018d8ff8785e" />

Le modèle de régression représente 48 % de la variance de la variable dépendante (y) qui provient de celles des variables indépendantes (X).

Le coefficient de détermination, R2 (R-carré) est le carré de la corrélation de Pearson entre valeurs prédites et vraies valeurs. Il mesure la qualité de l’ajustement d’un modèle de régression.
- R-carré = Variation expliquée (SCE)/ Variation totale (SCT)
- Le coefficient de détermination se situe entre 0 et 1.
Plus la variance expliquée par le modèle de régression est importante, plus les points de données se rapprocheront de la ligne de régression ajustée.

## Data Analysis
1. Compare two prediction methods:
   - a. A traditional logistic regression
   - b. A K-Means clustering, where centroids are used to make predictions.
2. Use confusion matrices for optimal model evaluation.

# Projet 10 (French)
Detectez des faux billets avec Python

OBJECTIFS
Détectez des faux billets avec Python

MISSION: Mettre en place une modélisation qui sérait capable d'identifier automatiquement les vraies des faux billets
1. Une analyse exploratoire et descriptive des données, réaliser la régression linéaire afin de combler des valeurs manquantes.
2. Mettre en concurrence 2 méthodes de prédiction : 
	- a.) Une régression logistique classique
	- b.) Un K-Means, duquel seront utilisés les centroïdes pour réaliser la prediction
3. Des matrices de confusion pour des évaluations optimales des modèles. 
