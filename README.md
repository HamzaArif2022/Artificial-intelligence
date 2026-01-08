# Mini Projet - Intelligence Artificielle 🤖


Ce projet contient deux tâches principales d'apprentissage automatique : régression linéaire et classification binaire.

---

## 📋 Structure du Projet

```
miniProjet/
├── tache1_regression_lineaire.ipynb    # Tâche 1: Régression Linéaire
├── tache2_classification_binaire.ipynb # Tâche 2: Classification Binaire
├── requirements.txt                     # Dépendances Python
└── README.md                           # Ce fichier
```

---

## 🎯 Objectifs du Projet

### **Tâche 1 : Régression Linéaire**
- Jeu de données : California Housing Prices (20,640 observations)
- Objectif : Prédire le prix médian des maisons
- Modèle : Régression linéaire simple
- Métriques : EQM, REQM, R²
- Visualisations : Graphiques de prédictions, résidus, importance des caractéristiques

### **Tâche 2 : Classification Binaire**
- Jeu de données : Breast Cancer Wisconsin (569 observations)
- Objectif : Classifier les tumeurs (maligne vs bénigne)
- Modèles : Régression Logistique & Arbre de Décision
- Métriques : Exactitude, Précision, Rappel, Score-F1
- Visualisations : Matrices de confusion, comparaison des modèles

---

## 🚀 Installation

### Prérequis
- Python 3.8 ou supérieur
- pip (gestionnaire de paquets Python)

### Installation des dépendances

#### Option 1 : Avec pip
```bash
pip install -r requirements.txt
```

#### Option 2 : Installation manuelle
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

---

## 💻 Utilisation

### Lancer Jupyter Notebook
```bash
jupyter notebook
```

Puis ouvrir :
- `tache1_regression_lineaire.ipynb` pour la Tâche 1
- `tache2_classification_binaire.ipynb` pour la Tâche 2

### Exécution des notebooks

1. Ouvrez le notebook souhaité dans Jupyter
2. Exécutez les cellules séquentiellement (Shift + Enter)
3. Les jeux de données sont chargés automatiquement via scikit-learn
4. Toutes les visualisations s'afficheront dans le notebook

---

## 📊 Résultats Attendus

### Tâche 1 - Régression Linéaire
- **R² attendu** : ~0.60 (60% de variance expliquée)
- **REQM** : Erreur moyenne sur le prix des maisons
- **Graphiques** :
  - Distribution de la variable cible
  - Matrice de corrélation
  - Prédictions vs valeurs réelles
  - Distribution des résidus
  - Droite de régression avec la caractéristique la plus importante

### Tâche 2 - Classification Binaire
- **Régression Logistique** : Exactitude ~97%
- **Arbre de Décision** : Exactitude ~94%
- **Graphiques** :
  - Distribution des classes
  - Histogrammes des caractéristiques par classe
  - Matrices de confusion
  - Comparaison des performances
  - Visualisation de l'arbre de décision
  - Importance des caractéristiques

---

## 📚 Jeux de Données Utilisés

### 1. California Housing (Tâche 1)
- **Source** : sklearn.datasets
- **Taille** : 20,640 exemples
- **Caractéristiques** : 8 variables (revenu médian, âge des maisons, nombre de pièces, etc.)
- **Cible** : Prix médian des maisons (en $100k)

### 2. Breast Cancer Wisconsin (Tâche 2)
- **Source** : sklearn.datasets
- **Taille** : 569 exemples
- **Caractéristiques** : 30 variables (caractéristiques des cellules tumorales)
- **Cible** : Diagnostic (0 = Maligne, 1 = Bénigne)

---

## 🛠️ Technologies Utilisées

| Bibliothèque | Version | Usage |
|--------------|---------|-------|
| **pandas** | ≥2.0.0 | Manipulation de données |
| **numpy** | ≥1.24.0 | Calculs numériques |
| **scikit-learn** | ≥1.3.0 | Apprentissage automatique |
| **matplotlib** | ≥3.7.0 | Visualisations |
| **seaborn** | ≥0.12.0 | Visualisations statistiques |
| **jupyter** | ≥1.0.0 | Environnement interactif |

---

## 📖 Contenu Détaillé

### Tâche 1 : Régression Linéaire

#### 1. Choix et description du jeu de données
- Présentation du jeu de données California Housing
- Contexte et objectif
- Description des caractéristiques

#### 2. Préparation des données
- Chargement du jeu de données
- Exploration et nettoyage
- Vérification des valeurs manquantes
- Visualisation de la distribution
- Matrice de corrélation
- Séparation caractéristiques/cible
- Division entraînement/test (80/20)

#### 3. Modélisation et évaluation
- Entraînement du modèle de régression linéaire
- Calcul des coefficients
- Prédictions
- Métriques : EQM, REQM, R²
- Visualisations multiples
- Analyse avec une caractéristique unique

#### 4. Interprétation des résultats
- Analyse des performances
- Discussion sur l'adéquation du modèle
- Limites et perspectives

---

### Tâche 2 : Classification Binaire

#### 1. Choix et description du jeu de données
- Présentation du jeu de données Breast Cancer
- Contexte médical
- Description des caractéristiques

#### 2. Préparation des données
- Chargement du jeu de données
- Exploration et nettoyage
- Distribution des classes
- Visualisation des caractéristiques
- Matrice de corrélation
- Standardisation des données
- Division entraînement/test stratifiée

#### 3. Modèles à tester

##### 3.1 Régression Logistique
- Entraînement
- Évaluation (Exactitude, Précision, Rappel, Score-F1)
- Rapport de classification
- Matrice de confusion

##### 3.2 Arbre de Décision
- Entraînement avec profondeur_max=5
- Évaluation complète
- Visualisation de l'arbre
- Importance des caractéristiques

#### 4. Comparaison et interprétation
- Tableau comparatif
- Visualisations comparatives
- Analyse du sur-apprentissage
- Discussion approfondie
- Recommandations

---

## 📝 Points Clés des Analyses

### Régression Linéaire
✅ Modèle simple et interprétable  
✅ Capture bien les tendances linéaires  
✅ R² de ~0.60 = performance acceptable  
⚠️ Limité pour les relations non-linéaires  

### Classification Binaire
✅ Régression Logistique : meilleur modèle (97% d'exactitude)  
✅ Excellente généralisation  
✅ Pas de sur-apprentissage significatif  
⚠️ Arbre de décision : léger sur-apprentissage malgré profondeur_max=5  

---

## 🎓 Concepts Abordés

- **Régression linéaire** : Modélisation de relations linéaires
- **Classification binaire** : Problèmes à deux classes
- **Prétraitement** : Nettoyage, encodage, standardisation
- **Division entraînement/test** : Validation des modèles
- **Métriques d'évaluation** : EQM, R², Exactitude, Précision, Rappel, Score-F1
- **Visualisation de données** : Graphiques exploratoires et de résultats
- **Sur-apprentissage** : Détection et prévention du sur-apprentissage
- **Comparaison de modèles** : Analyse critique des performances

---

## 🔧 Troubleshooting

### Erreur d'importation
```bash
ModuleNotFoundError: No module named 'sklearn'
```
**Solution** : Installez scikit-learn
```bash
pip install scikit-learn
```

### Problème avec matplotlib
```bash
ImportError: cannot import name '_path' from 'matplotlib'
```
**Solution** : Réinstallez matplotlib
```bash
pip install --upgrade matplotlib
```

### Jupyter ne démarre pas
**Solution** : Vérifiez l'installation
```bash
pip install --upgrade jupyter
jupyter --version
```

---

## 📧 Contact

Pour toute question sur ce projet, contactez votre instructeur ou consultez la documentation des bibliothèques utilisées :

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Seaborn Documentation](https://seaborn.pydata.org/)

---

## 📄 Licence

Ce projet est réalisé dans le cadre du cours d'Intelligence Artificielle - Cycle d'ingénieur (2025/2026).

---

**Bon apprentissage ! 🚀**




