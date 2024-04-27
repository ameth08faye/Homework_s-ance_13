# Homework_s-ance_13

Dans l'exposé sur traitement statistique des valeurs manquantes et aberrantes avec R, voici ce que j'ai retenu essentiellement
I. Approches pour traiter les valeurs manquantes
Types de valeurs manquantes :
MCAR (Manquantes Complètement Aléatoires) : Dans ce cas, les données manquent de manière totalement aléatoire, sans lien avec d’autres variables.
MAR (Manquantes Aléatoires Conditionnelles) : Les données manquent en relation avec d’autres variables observées, mais pas directement en lien avec les valeurs manquantes elles-mêmes.
MNAR (Manquantes Non Aléatoires) : Ici, les données manquent en relation avec des variables non observées, ce qui rend leur traitement plus complexe.
Méthodes de traitement des valeurs manquantes :
Suppression : Cette méthode consiste à éliminer les observations incomplètes. Elle est simple, mais peut entraîner une perte significative de données.
Imputation par la moyenne : On remplace les valeurs manquantes par la moyenne des observations disponibles. C’est adapté pour les données où la variabilité est faible.
Imputation par la médiane : Utilisée lorsque les données sont asymétriques, cette méthode remplace les valeurs manquantes par la médiane pour plus de robustesse.
Imputation par régression : Plus sophistiquée, elle utilise un modèle de régression pour prédire les valeurs manquantes à partir d’autres variables.
Imputation par HOT DECK : On remplace les valeurs manquantes par des valeurs similaires provenant d’autres observations dans le jeu de données.
Imputation par KNN (k-plus proches voisins) : Cette méthode impute les valeurs manquantes en se basant sur les moyennes des k observations les plus proches.
LOCF (Last Observation Carried Forward) : Utilisée dans les séries chronologiques, elle propage la dernière observation disponible.

II. Traitement des valeurs aberrantes
Détection des valeurs aberrantes :
Détection par domaine de valeurs : Identifie les aberrations en se basant sur les intervalles attendus pour certaines variables.
Détection graphique : Utilisation de graphiques comme les boxplots et les nuages de points pour visualiser et identifier les anomalies.
Méthode de Tukey (IQR) et Score Z : Détectent les valeurs extrêmes en utilisant des mesures statistiques de dispersion.
Méthodes de traitement :
Suppression : Élimination des valeurs aberrantes, adaptée pour les erreurs de saisie ou les données avec faible effectif.
Transformation : Techniques comme la transformation logarithmique pour minimiser l'influence des extrêmes, ou la winsorisation qui limite les valeurs à un certain percentile pour conserver plus de données.




Dans l'exposé sur l'ANOVA et les tests non paramétriques, voici ce que j'ai retenu essentiellement:

I. Analyse de la variance (ANOVA)
Développement et Application : L’ANOVA, développée par Ronald Fisher au début du 20ème siècle, permet de détecter les différences ou similitudes dans une population étudiée. Elle se concentre sur l’interaction entre les facteurs de variabilité et une variable quantitative principale.
Exemple Pratique : Prenons l’exemple des scores attribués par différents correcteurs lors d’olympiades de mathématiques. L’ANOVA nous permet d’analyser l’influence du correcteur et du sexe des candidats sur les notes.
Limitations : L’ANOVA suppose l’égalité des variances et une distribution normale des données. Elle est également sensible aux valeurs aberrantes, nécessitant souvent des tests post-hoc pour identifier les groupes spécifiquement différents.

II. Tests Non Paramétriques
Définition et Utilité : Contrairement à l’ANOVA, les tests non paramétriques ne requièrent pas d’hypothèse sur la distribution des données. Ils sont utilisés pour des données qui ne suivent pas une distribution spécifique, en utilisant des statistiques d’ordre ou des tableaux de contingence.
Exemples de Tests :
Test de Wilcoxon : Compare les distributions de jeux de variables appariées en prenant en compte les signes et amplitudes des différences.
Test du khi-carré : Évalue si une distribution de fréquences observées diffère de celle attendue. Il est souvent utilisé pour des données catégorielles.
Test U de Mann-Whitney : Compare les rangs de deux groupes pour tester s’ils proviennent de la même population.
Test de Kruskal-Wallis : C’est une extension du test U de Mann-Whitney pour plus de deux groupes, permettant de détecter des différences dans la distribution des échantillons.

III. Applications Pratiques Des liens pour ouvrir des fichiers R d’application de l’ANOVA et des tests non paramétriques sont mentionnés, ce qui vous permettra de mettre en pratique directement les méthodes étudiées.




Dans l'exposé sur les statistiques descriptives et la visualisation des variables catégorielles avec ggplot2, voici ce que j'ai retenu essentiellement:

I. Types de Variables dans R
Les types de variables manipulées en R sont introduits, et on les distingue entre :
Variables quantitatives (discrètes et continues) : Ces variables prennent des valeurs numériques et peuvent être mesurées avec précision.
Variables qualitatives (nominales et ordinales) : Ces variables représentent des catégories ou des groupes et ne sont pas mesurées numériquement.
En R, les variables sont souvent gérées sous forme de vecteurs, incluant les types tels que double, float, character, et surtout les factors, qui sont des vecteurs de valeurs prédéfinies.

II. Visualisation des Données avec ggplot2
Grammaire graphique : ggplot2, fondé par Hadley Wickham, est basé sur la grammaire graphique. Cette approche aide à construire des graphiques de manière logique en mélangeant différentes couches d’information visuelle.
Composantes de ggplot2 :
aes (Esthétique) : Cette composante définit comment les variables sont mappées aux propriétés visuelles telles que la couleur, la forme et la taille des points ou des lignes sur un graphique.
geom_ functions : Ces fonctions déterminent le type de graphique (barres, lignes, points, etc.). Par exemple, geom_bar() pour des graphiques à barres et geom_point() pour des nuages de points.
labs et theme : Ces éléments permettent de personnaliser les titres, légendes et autres éléments esthétiques du graphique.
scale_ functions : Elles contrôlent l’échelle des esthétiques, comme la couleur et la taille, permettant des ajustements précis sur la représentation visuelle.


