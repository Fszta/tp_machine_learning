# TP Machine learning

- Le TP sera réalisé dans un notebook python (google collab ou jupyter...)
- Il sera uploadé sur git et le lien transmis à votre encadrant


## Avant de commencer
- Téléchargez le jeu de donnée, <a href="https://we.tl/t-bUuW1b7Wsv">disponible ici</a>

## Informations
Pour ce tp vous allez utiliser les librairies suivantes: 
- scikit-learn
- pandas
- matplotlib et / ou seaborn

> Naturellement, vous pouvez utiliser toutes les librairies que vous voulez, les précédentes sont listées à titre informatif.


## Partie 1 : Analyse Exploratoire des Données (EDA)
<b>Objectif : Comprendre les données et leur structure, identifier les patterns et les problèmes potentiels.</b>

### 1.1 Vue d'ensemble des données :

Charger le jeu de données dans un dataframe pandas et afficher les premières lignes.

<b>Questions :</b>
- Quelles sont les différentes colonnes du jeu de données ?
- Combien y a-t-il d'entrées dans le jeu de données ?
- Le jeu de données contient-il des valeures nulles ? Si oui combien ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

### 1.2 Statistiques descriptives :

Générer des statistiques descriptives pour le jeu de données.
<b>Questions :</b>
- Quelle est la moyenne d'âge, de taille et de poids des fumeurs ?
- Y a-t-il des motifs ou des valeurs aberrantes notables dans les données ? (Un age 200 ans par exemple)
- Quelle est l'écart type de l'hémoglobine ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

### 1.3 Distribution de la donnée :
question
- Combien y a-il de fumeur vs non-fumeur ? Le résultat doit être présenté sous forme de "pie chart"
- Combien d'hommes? sont fumeurs ? Combien de femmes ? Afficher un histogramme
- Quelle est la moyenne d'age des hommes fumeurs ?


### 1.4 Analyse de corrélation :

Calculer et visualiser la matrice de corrélation, le but étant d'étudier la corrélation des variables entre elles.
<b>Questions :</b>
- Quel problème rencontrez-vous ?
- Passez à la partie 2 et revenez aux questions suivante plus tard.

- Quelles variables sont les plus fortement corrélées entre elles ?
- Comment la variable cible (fumeur) est-elle corrélée avec les autres variables ? Donnez le top 3

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

## Partie 2 : Data pre-processing
Objectif : Préparer les données en traitant les valeurs manquantes, en encodant les variables catégorielles et en normalisant les variables numériques.

### 2.1 Gestion des Valeurs Manquantes :

Décider d'une stratégie pour gérer les valeurs manquantes (par exemple, suppression, estimation).
Implémenter la stratégie choisie.

<b>Questions :</b>
- Quelle méthode avez-vous choisie pour gérer les valeurs manquantes et pourquoi ?
- Comment cette méthode impacte-t-elle les données ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

## 2.2 Encodage des catégories

Encodez les variables en utilisant un <a href="https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html">OneHotEncorer</a>
- tartare
- gender
- oral

<b>Questions :</b>
- Quel autre traitement de la donnée pourriez-vous faire pour optimiser l'entraînement ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.


## Partie 3 : 

<b>Objectif : Choisir et entraîner plusieurs modèles de classification, ajuster les hyperparamètres et comparer les performances des modèles.</b>

### 3.1 Création de jeu de test et d'entraînement

Séparez la data en 2 parties : train & test.
 
<b>Questions :</b>
- Quelle proportion des données avez-vous utilisée pour l'entraînement et pour le test ?
- Pourquoi est-il important de diviser les données ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

### 3.2 Entraînement d'un modèle simple : LogisticRegression

Entraîner un modèle de régression logistique simple sur les données d'entraînement.
<b>Questions :</b>
- Quels sont les résultats de ce modèle sur le jeu de test  ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.


### 3.3 Entraîner et ajuster les paramètres de plusieurs modèles
Entraîner au moins quatre modèles différents et ajuster leurs hyperparamètres en utilisant GridSearchCV.
> Modèles suggérés : Arbre de décision, KNN, Random forest, SVM, xgboost.
> Pour le tuning des hyperparamètres, pensez au <a href="https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html">gridsearch</a> et <a href="https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html">randomsearch</a>

<b>Questions :</b>
- Quels hyperparamètres avez-vous ajustés pour chaque modèle ?
- Quel est l'impact de l'ajustement des hyperparamètres sur les performances des modèles ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.

### 3.4 Évaluer les Performances des Modèles
Évaluer chaque modèle en utilisant des métriques telles que l'accuracy, le recall, le F1-score, afficher le nombre de faux-positifs...

<b>Questions :</b>
- Quelle est la performance de chaque modèle sur l'ensemble de test ?
- Quel modèle a les meilleures performances globales et pourquoi ?

> Appelez votre encadrant pour validation, vous pouvez continuer en attendant son arrivée.
