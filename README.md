1. Contexte du projet
Dans le cadre de cet appel à projet, nous avons travaillé sur la base de données Open Food Facts. L’objectif est de vérifier si les informations disponibles permettent d’envisager une application capable de prédire la note nutritionnelle (nutrition_grade_fr) des produits, et d’identifier les facteurs les plus déterminants dans cette prédiction.

2. Démarche méthodologique
a. Nettoyage des données
Suppression des doublons et des colonnes non pertinentes

Identification et traitement des valeurs manquantes :

Suppressions (quand la donnée est indispensable)

Imputations métier (valeurs logiques pour certains produits)

Remplissage par moyenne/médiane

Traitement des valeurs aberrantes :

Analyse visuelle (boxplots, distribution)

Seuils métiers appliqués (ex : pas plus de 100g de sucre pour 100g)

Respect des principes RGPD : la base ne contient aucune donnée personnelle

b. Analyse exploratoire
Analyse univariée :

Description des distributions (moyenne, médiane, quantiles)

Visualisations : histogrammes, boxplots

Analyse multivariée :

Corrélations entre variables (heatmap, scatterplots)

ACP pour synthétiser l’information et détecter les variables explicatives principales

ANOVA pour valider la significativité des différences entre les groupes nutritionnels

3. Résultats principaux
La majorité des produits sont notés D et E, traduisant une qualité nutritionnelle globalement faible.

Les variables energy_100g et sugars_100g sont les plus fortement corrélées à la note nutritionnelle, confirmées par l'ACP et les tests ANOVA.

L’ACP permet de visualiser l’importance relative des variables et leur contribution à la discrimination des groupes nutritionnels.

Les tests statistiques (p-value < 0,05) confirment que les différences entre les groupes sont significatives pour toutes les variables nutritionnelles.

4. Conclusion
Les variables nutritionnelles disponibles dans la base Open Food Facts permettent bien de distinguer les produits selon leur qualité nutritionnelle.

Le projet valide la faisabilité d’une application capable de prédire la note nutrition_grade_fr.

La base, une fois nettoyée, est exploitable et conforme au RGPD.

5. Fichiers disponible sur demande
Nom_Prenom_1_notebook_mmaaaa.ipynb : traitements + analyses

Nom_Prenom_2_presentation_mmaaaa.pdf : support de soutenance disponible

6. Environnement
Python 3.10

Librairies : pandas, numpy, seaborn, matplotlib, scikit-learn, scipy

