## Machine Learning sur les marchés financiers (SPY)

## Objectif du projet
Ce projet a pour objectif de prédire la direction du marché boursier (hausse ou baisse) à partir de données historiques de l’indice SPY, en utilisant différentes méthodes de machine learning.

L’étude compare plusieurs modèles allant de la régression logistique aux réseaux de neurones.

## Données utilisées
Les données proviennent de Yahoo Finance via la librairie `yfinance`.

- Actif : SPY (ETF S&P 500)
- Période : 2015 - 2023
- Variables : prix de clôture, volume

## Feature engineering
Des variables explicatives ont été construites :

- Rendement journalier
- Volatilité (rolling window)
- Moyenne mobile
- Momentum
- Variation du volume
- Interactions entre variables

## Modèles testés

Plusieurs modèles de machine learning ont été comparés :

- Régression logistique
- Random Forest
- Réseau de neurones (Keras)

## Résultats

Les performances obtenues sont proches du hasard (~50%), ce qui montre la difficulté du problème :

- Logistic Regression ≈ 49%
- Random Forest ≈ 50%
- Neural Network ≈ 51%

## Analyse

- Les marchés financiers sont très bruités
- Faible corrélation entre features et target
- Risque élevé de surapprentissage
- Les modèles simples et complexes ont des performances similaires

## Expériences réalisées

- Ajout d’interactions entre variables
- Optimisation des hyperparamètres
- Comparaison biais / variance
- Étude du surapprentissage


##  Conclusion

Ce projet montre que la prédiction des marchés financiers avec des modèles classiques de machine learning est très difficile.

Même les modèles complexes (réseaux de neurones) n’apportent pas d’amélioration significative.
 Le Random Forest reste le meilleur compromis en termes de robustesse.


## Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- yfinance

## Auteur
Projet réalisé dans le cadre d’un TP de Machine Learning.
