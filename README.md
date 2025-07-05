
# Projet d’analyse de données nutritionnelles — Open Food Facts & Santé publique France

## Présentation

Ce projet s’inscrit dans le cadre de la formation Data Scientist. Il a été mené pour répondre à une mission confiée par l’agence Santé publique France. L’objectif est d’évaluer la qualité des données de la base Open Food Facts, afin d’étudier la faisabilité d’une application de suggestion de valeurs nutritionnelles manquantes pour aider les usagers à remplir la base plus efficacement.

## Objectif

L’objectif est de vérifier si les informations disponibles dans la base Open Food Facts permettent :
- de nettoyer et structurer efficacement les données en vue d’une exploitation fiable ;
- d’envisager une application capable de suggérer la note nutritionnelle (nutrition_grade_fr) des produits ;
- d’identifier les facteurs les plus déterminants dans cette prédiction ;
- de produire des visualisations lisibles pour un public non-expert ;
- de garantir le respect du RGPD (aucune donnée personnelle traitée).

## Compétences mobilisées

- **Collecte et filtrage de données** : nettoyage des doublons et des colonnes inutiles.
- **Traitement des valeurs manquantes** : suppression, imputation par logique métier ou statistiques (moyenne, médiane).
- **Traitement des valeurs aberrantes** : visualisation (boxplots, histogrammes) et seuils métiers.
- **Analyse univariée et bivariée** : statistiques descriptives, tests statistiques, visualisations (diagrammes variés).
- **Analyse multivariée** : analyse en composantes principales (ACP), corrélations, ANOVA.
- **Visualisation des données** : production de graphiques lisibles pour un public néophyte.
- **Respect du RGPD** : conformité aux 5 principes fondamentaux.
- **Conception de recommandations métier** : interprétation des résultats pour guider les décisions de Santé publique France.

## Résultats principaux

- La majorité des produits sont notés D ou E, indiquant une qualité nutritionnelle globalement faible.
- Les variables `energy_100g` et `sugars_100g` sont les plus fortement corrélées à la note nutritionnelle.
- L’ACP confirme que ces variables expliquent une grande partie de la variance des notes.
- Les tests statistiques (p-value < 0.05) confirment la significativité des différences entre les groupes nutritionnels.
- La base, une fois nettoyée, est exploitable pour le développement d’une application de prédiction.

## Livrable

Le livrable principal est une présentation en PDF illustrant la méthodologie, les visualisations de données, les résultats, les tests statistiques et les recommandations formulées à Santé publique France.

## Données

Source : [Open Food Facts — off.fr](https://world.openfoodfacts.org/)

## Auteure

**Oumou Faye**  
Formation : Data Scientist  
Mentor : Medina Hadjem

