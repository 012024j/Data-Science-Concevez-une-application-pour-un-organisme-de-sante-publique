1. Contexte du projet
Dans le cadre de ce projet, nous avons travaillé sur la base de données Open Food Facts.
L’objectif est de vérifier si les informations disponibles permettent d’envisager une application capable de prédire la note nutritionnelle (nutrition_grade_fr) des produits, et d’identifier les facteurs les plus déterminants dans cette prédiction.

2. Démarche méthodologique
a. Nettoyage des données
Suppression des doublons et des colonnes non pertinentes

Identification et traitement des valeurs manquantes :

Suppression (lorsque la donnée est indispensable)

Imputation par logique métier (ex. : 0g de protéines pour un produit composé uniquement de sucre)

Remplissage par moyenne ou médiane

Traitement des valeurs aberrantes :

Analyse visuelle (boxplots, distributions)

Seuils métiers appliqués (ex. : pas plus de 100g de sucre pour 100g)

Respect du RGPD : la base ne contient aucune donnée personnelle

b. Analyse exploratoire
Analyse univariée :

Statistiques descriptives (moyenne, médiane, quantiles)

Visualisations : histogrammes, boxplots

Analyse multivariée :

Corrélations entre variables (matrice de corrélation, scatterplots)

ACP pour réduire la dimensionnalité et identifier les variables explicatives

ANOVA pour tester la significativité des différences entre les groupes nutritionnels

3. Résultats principaux
La majorité des produits sont notés D et E, traduisant une qualité nutritionnelle globalement faible.

Les variables energy_100g et sugars_100g sont les plus fortement corrélées à la note nutritionnelle, ce que confirment l’ACP et les tests ANOVA.

L’ACP met en évidence la contribution relative des variables à la discrimination entre les groupes.

Les tests statistiques (p-value < 0.05) confirment que les différences entre les groupes sont significatives pour toutes les variables nutritionnelles.

4. Conclusion
Les variables nutritionnelles disponibles dans la base Open Food Facts permettent de distinguer les produits selon leur qualité nutritionnelle.

Le projet confirme la faisabilité d’un outil de prédiction de la note nutrition_grade_fr.

Une fois nettoyée, la base est exploitable et conforme au RGPD.


5. Environnement
Python 3.10

Librairies : pandas, numpy, seaborn, matplotlib, scikit-learn, scipy

Auteure
Oumou Faye
Formation : Data Scientist
Mentor : Medina Hadjem