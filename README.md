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

3. Identified outliers <img width="959" alt="aaa" src="https://github.com/user-attachments/assets/e47bbb28-d062-47ba-82ff-065c1a87e949" />


## Exploratory Data Analysis (EDA)
Conduct an exploratory and descriptive data analysis
1. Checked the distribution of the data

<img width="947" alt="aaa" src="https://github.com/user-attachments/assets/6a21cf1b-14ed-409e-8124-f89b72576961" />

2. Correlation

<img width="867" alt="aa" src="https://github.com/user-attachments/assets/3ceae67f-87c0-4c5f-9ae7-30533d791d88" />


3. Used linear regression to impute missing values.

Linear Regression

<img width="973" alt="aaaa" src="https://github.com/user-attachments/assets/dc4881da-9782-47a8-baa1-018d8ff8785e" />

Le modèle de régression représente 48 % de la variance de la variable dépendante (y) qui provient de celles des variables indépendantes (X).

Le coefficient de détermination, R2 (R-carré) est le carré de la corrélation de Pearson entre valeurs prédites et vraies valeurs. Il mesure la qualité de l’ajustement d’un modèle de régression.
- R-carré = Variation expliquée (SCE)/ Variation totale (SCT)
- Le coefficient de détermination se situe entre 0 et 1.
Plus la variance expliquée par le modèle de régression est importante, plus les points de données se rapprocheront de la ligne de régression ajustée.

<img width="1094" alt="aaaaaaaa" src="https://github.com/user-attachments/assets/89cc3062-7dde-49a2-bcc9-28d050764f44" />

Predicted missing values

<img width="1169" alt="aaaaaaa" src="https://github.com/user-attachments/assets/8d130660-5193-4bdc-9209-ac91964c8aec" />

<img width="1169" alt="aaaaaaa" src="https://github.com/user-attachments/assets/42600043-1660-4d33-841a-29d250cc8633" />


## Data Analysis
1. Compare two prediction methods:
- Traditional logistic regression

<img width="1290" alt="aaaaaa" src="https://github.com/user-attachments/assets/d813e7aa-2be6-4251-a1d9-301159ccdede" />

<img width="1003" alt="aa" src="https://github.com/user-attachments/assets/fe6a1df6-456b-49ae-8e97-e86b261b6914" />


- K-Means clustering, where centroids are used to make predictions.

<img width="1007" alt="aa" src="https://github.com/user-attachments/assets/8046ae03-0d37-4cd1-906f-421ce8ba1dc5" />

<img width="1187" alt="aaa" src="https://github.com/user-attachments/assets/62d57da3-fe84-4e03-998c-88b70708c6a8" />

<img width="1089" alt="aaaaa" src="https://github.com/user-attachments/assets/8d100846-5092-451b-bf50-a38e16960997" />


2. Use confusion matrices for optimal model evaluation.
<img width="942" alt="aaa" src="https://github.com/user-attachments/assets/2fa578f6-9910-460d-8b15-4b309902ef65" />

## Insights and Results
- Applying the logistic regression model to the 'billets_production' data: The classification of each banknote gives the probability that a banknote is genuine or counterfeit.
A probability greater than or equal to 0.5 indicates a genuine banknote.
A probability less than 0.5 is considered a counterfeit banknote.

<img width="1166" alt="aa" src="https://github.com/user-attachments/assets/8f2b897f-3858-442b-a598-10c94ef819c0" />

- Applying the k-means model to the 'billets_production' data: The k-means algorithm allows us to calculate the centers of sample partitions, called "centroids," iteratively by minimizing the distance between points within a partition and maximizing the distance between partitions until the centroids no longer change significantly, or after a number of iterations fixed in advance.
  
<img width="1259" alt="aaa" src="https://github.com/user-attachments/assets/04e1edaa-7d0f-42b2-be28-f24c4fc197a1" />

## Recommendation
The prediction by the logistic regression model is more stable and performs better than the prediction by the k-Means model.



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
