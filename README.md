# Mini-Projet : Apprentissage Supervisé Linéaire
## Module : Machine Learning
## Année universitaire : 2026

---

## 👤 Informations de l’étudiant
- **Nom et Prénom** : Sidi Med Med Lemine
- **Matricule** : C34646
- **Niveau** : Master 1 Intelligence Artificielle (M1 IA)
- **Université** : Faculté des Sciences et Techniques (FST)

---

## 🎯 Objectif du Mini-Projet
L’objectif de ce mini-projet est de consolider les bases de l’apprentissage supervisé
à travers l’implémentation complète et l’analyse de deux modèles fondamentaux :

- **MLS (Machine Learning Supervisé)** : Régression Linéaire  
- **MLNS (Classification Supervisée)** : Régression Logistique  

Le projet couvre toutes les étapes classiques d’un pipeline de Machine Learning :
préparation des données, implémentation des algorithmes, entraînement,
évaluation et interprétation des résultats.

---

## 🧩 Structure du Dépôt
SidiMedMedLemine_C34646_2026_MachineLearning/
│
├── Mini_Projet_ML_2026_AMOUNT.ipynb
├── README.md
└── dataset/
└── Insurance.csv

---

## 🟦 PARTIE 1 : RÉGRESSION LINÉAIRE (MLS)

### 🔹 Dataset utilisé
- **Nom du fichier** : `Insurance.csv`
- **Source** : Kaggle (dataset d’assurance)
- **Variables disponibles** :
  - `Age`
  - `Policy Term`
  - `PPT`
  - `Plan` (catégorielle)
  - **`Amount`** (variable cible numérique)

### 🔹 Problème traité
Prédire le **montant (`Amount`)** à partir des caractéristiques de l’assuré.

---

### 🔹 Étapes d’implémentation de l’algorithme

1. **Chargement des données**
   - Import du fichier CSV depuis Google Drive
   - Vérification des colonnes et des types de données

2. **Prétraitement**
   - Nettoyage des noms de colonnes
   - Conversion de la variable cible `Amount` en type numérique
   - Suppression des valeurs manquantes si nécessaire

3. **Encodage**
   - Transformation des variables catégorielles (ex : `Plan`)
   - Utilisation de `get_dummies()` avec suppression de la première modalité

4. **Analyse exploratoire**
   - Calcul de la matrice de corrélation
   - Visualisation via une **Heatmap**

5. **Formalisation du modèle**
   - Modèle de régression linéaire :
     \[
     y = \beta_0 + \sum_{i=1}^{n} \beta_i x_i + \varepsilon
     \]

6. **Séparation des données**
   - 80 % pour l’entraînement
   - 20 % pour le test

7. **Implémentation de l’algorithme**
   - Entraînement du modèle de **Régression Linéaire**

8. **Prédiction**
   - Prédiction des valeurs de `Amount` sur l’ensemble de test

9. **Évaluation**
   - Calcul de l’Erreur Quadratique Moyenne (**MSE**)
   - Calcul du Coefficient de Détermination (**R²**)

10. **Interprétation**
    - Analyse des coefficients βᵢ
    - Étude de l’influence de chaque variable sur le montant prédit

---

### 🔹 Algorithme utilisé
- **Régression Linéaire (Machine Learning Supervisé – MLS)**

---

## 🟩 PARTIE 2 : RÉGRESSION LOGISTIQUE (MLNS)

### 🔹 Dataset utilisé
- **Nom** : Iris Dataset
- **Source** : scikit-learn
- **Type de problème** : Classification binaire (Classe 0 vs Autres)

---

### 🔹 Étapes d’implémentation de l’algorithme

1. **Chargement du dataset Iris**
   - Utilisation de `load_iris()` depuis scikit-learn

2. **Préparation des données**
   - Séparation des variables d’entrée (X) et de la cible (y)
   - Transformation du problème multi-classes en **classification binaire**

3. **Normalisation**
   - Standardisation des variables avec `StandardScaler`

4. **Séparation Train / Test**
   - 80 % entraînement / 20 % test

5. **Implémentation de l’algorithme**
   - Entraînement du modèle de **Régression Logistique**

6. **Modélisation probabiliste**
   - Fonction sigmoïde :
     \[
     P(y=1|x) = \frac{1}{1 + e^{-z}}
     \]

7. **Évaluation**
   - Construction de la **Matrice de Confusion**
   - Calcul des métriques :
     - Accuracy
     - Precision
     - Recall

---

### 🔹 Algorithme utilisé
- **Régression Logistique (Classification supervisée – MLNS)**

---

## 📊 Résultats et Analyse
- La régression linéaire permet de prédire efficacement une variable continue
  et d’interpréter l’importance des variables explicatives.
- La régression logistique permet de modéliser une probabilité d’appartenance
  à une classe et d’évaluer les performances à l’aide de métriques adaptées.

---

## ✅ Conclusion
Ce mini-projet a permis d’implémenter pas à pas deux algorithmes fondamentaux
du Machine Learning Supervisé. Il a renforcé la compréhension du pipeline
complet, depuis les données brutes jusqu’à l’interprétation des résultats.

---

## 🛠️ Outils utilisés
- Python
- Google Colab
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn

