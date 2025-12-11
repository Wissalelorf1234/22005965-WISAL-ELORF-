



WISSAL ELORF 



![Ma photo](https://raw.githubusercontent.com/Wissalelorf1234/22005965-WISAL-ELORF-/main/nom_image.jpg)



# Compte Rendu : Analyse Exploratoire du Jeu de Données Iris

---

## 1. Introduction

Ce compte rendu présente une analyse exploratoire du célèbre jeu de données Iris, qui contient des mesures morphologiques de trois espèces de fleurs d'iris (Setosa, Versicolor et Virginica).

---

## 2. Objectifs de l'Analyse

- Explorer la structure et la composition du jeu de données
- Examiner les distributions des variables numériques
- Identifier les relations entre les caractéristiques
- Détecter d'éventuelles valeurs aberrantes
- Comparer les statistiques descriptives entre les espèces

---

## 3. Description des Données

### 3.1 Structure du Dataset

Le jeu de données Iris comprend :

- **150 observations** (50 par espèce)
- **4 variables numériques** : longueur et largeur des sépales et pétales (en cm)
- **1 variable catégorielle** : l'espèce (setosa, versicolor, virginica)

### 3.2 Variables Étudiées

| Variable | Description |
|----------|-------------|
| `sepal length (cm)` | Longueur du sépale |
| `sepal width (cm)` | Largeur du sépale |
| `petal length (cm)` | Longueur du pétale |
| `petal width (cm)` | Largeur du pétale |
| `species` | Espèce de la fleur |

---

## 4. Méthodologie

L'analyse a été réalisée en Python avec les bibliothèques suivantes :

- **Pandas** : manipulation des données
- **Seaborn & Matplotlib** : visualisations
- **Scikit-learn** : chargement du dataset

---

## 5. Résultats de l'Analyse

### 5.1 Statistiques Descriptives Globales

Les statistiques descriptives révèlent :

- Les longueurs de sépales varient de **4.3 à 7.9 cm**
- Les largeurs de sépales varient de **2.0 à 4.4 cm**
- Les longueurs de pétales varient de **1.0 à 6.9 cm**
- Les largeurs de pétales varient de **0.1 à 2.5 cm**

### 5.2 Distribution des Variables

Les histogrammes avec courbes de densité (KDE) permettent d'observer :

- Des distributions parfois **bimodales ou multimodales**, suggérant des différences entre espèces
- Une variabilité importante dans les mesures de pétales

### 5.3 Détection des Valeurs Aberrantes

Les boxplots horizontaux montrent :

- Quelques valeurs aberrantes potentielles dans certaines variables
- Une dispersion variable selon les caractéristiques

### 5.4 Relations entre Variables

Le pairplot (matrice de nuages de points) révèle :

- Une **séparation claire** de l'espèce Setosa par rapport aux autres
- Des **chevauchements** entre Versicolor et Virginica
- Les dimensions des pétales sont particulièrement discriminantes

### 5.5 Corrélations

La matrice de corrélation indique :

- **Forte corrélation positive** entre longueur de pétale et largeur de pétale
- **Forte corrélation positive** entre longueur de pétale et longueur de sépale
- **Corrélation négative faible** entre largeur de sépale et longueur de pétale

### 5.6 Comparaison par Espèce

#### Setosa

- Pétales les plus petits (longueur et largeur)
- Sépales plus larges en moyenne

#### Versicolor

- Dimensions intermédiaires
- Caractéristiques se chevauchant avec Virginica

#### Virginica

- Pétales et sépales les plus grands
- Plus grande variabilité dans les mesures

---

## 6. Conclusions

L'analyse exploratoire du jeu de données Iris démontre que :

1. Les **dimensions des pétales** sont les caractéristiques les plus discriminantes pour différencier les espèces
2. L'espèce **Setosa est facilement séparable** des deux autres
3. Les espèces **Versicolor et Virginica présentent plus de similarités** et sont plus difficiles à distinguer
4. Les données sont de **bonne qualité** avec peu de valeurs aberrantes
5. Les **corrélations entre variables** suggèrent une redondance d'information qui pourrait être exploitée en modélisation

---

## 7. Perspectives

Ces résultats suggèrent que :

- Un modèle de classification pourrait efficacement prédire les espèces
- La réduction de dimensionnalité (ex: ACP) pourrait être intéressante
- Les dimensions des pétales devraient être privilégiées comme features principales

---

**Analyse réalisée le** : [Date]  
**Outils utilisés** : Python 3.x, Pandas, Seaborn, Matplotlib, Scikit-learn
