# Analyse de Segmentation et Prédiction de Valeur (CLV) pour Olist

## 1. Le Problème Business
Le département marketing de la marketplace Olist a un budget limité et cherche à optimiser ses dépenses. Pour cela, ils ont besoin de comprendre en profondeur leur base de clients :

Qui sont nos meilleurs clients ? (Champions)

Qui sont les clients "à risque" ou "perdus" ?

Sur quels clients devrions-nous concentrer nos efforts marketing pour maximiser le revenu futur ?

## 2. L'Objectif Analytique (Le Plan en 2 Phases)
Ce projet vise à fournir une stratégie de segmentation actionnable, basée sur la donnée.

Phase A : Segmentation RFM (SQL)

Construire une table "maître" au niveau client en joignant 8 tables (commandes, produits, clients...) via SQL.

Calculer les scores de Récence, Fréquence et Monétaire (RFM) pour chaque client.

Créer des segments clairs (ex: "Champions", "Clients à Risque", "Nouveaux").

Phase B : Modélisation Prédictive (Python & Scikit-learn)

Utiliser la table "maître" de la Phase A comme base pour le "feature engineering".

Construire un modèle de Régression (Linéaire ou Random Forest) pour prédire la Customer Lifetime Value (CLV) future (ou la probabilité de prochain achat).

## 3. Les Données
Source : [Olist E-Commerce Dataset (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Format : Une base de données relationnelle simulée (~100k commandes) répartie sur 8 fichiers CSV principaux (ex: orders, customers, order_items, products...).

## 4. La Stack Technique (Nos Outils)
Base de Données : SQLite (pour charger nos 8 CSV et pratiquer le SQL avancé).

Analyse & Modélisation : Python (Pandas, Scikit-learn).

Dashboarding & Storytelling : Tableau.