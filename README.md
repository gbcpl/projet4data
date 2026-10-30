# Projet 4 - Réaliser une étude de santé publique avec Python

## Présentation du projet

Ce projet, réalisé dans le cadre de ma formation de Data Analyst, consiste à mener une étude de santé publique à partir de données internationales portant sur la population, la disponibilité alimentaire, l'aide alimentaire et la sous-nutrition.

L'objectif est d'exploiter plusieurs sources de données pour mieux comprendre les enjeux de sécurité alimentaire à l'échelle mondiale, de calculer des indicateurs pertinents et de mettre en évidence des disparités entre les pays.

Cette étude mobilise Python pour préparer, analyser et croiser les données, ainsi que des outils de visualisation pour représenter les résultats et faciliter leur interprétation.

## Objectifs

- Explorer plusieurs jeux de données issus de sources internationales.
- Préparer et harmoniser les données afin de permettre leur exploitation conjointe.
- Analyser la situation mondiale en matière de sous-nutrition.
- Calculer la proportion de personnes en situation de sous-nutrition par rapport à la population.
- Étudier les disponibilités alimentaires et leurs différentes composantes.
- Comparer les situations entre les pays.
- Produire des visualisations pour communiquer les principaux résultats de l'étude.

## Sources de données

L'analyse s'appuie sur quatre jeux de données :

| Jeu de données | Utilisation |
|---|---|
| Population | Étudier la population des pays et disposer d'une base de comparaison pour les indicateurs démographiques. |
| Disponibilité alimentaire | Analyser les disponibilités alimentaires, les quantités destinées à la consommation humaine et animale, les pertes, les importations et les exportations. |
| Aide alimentaire | Étudier les données relatives à l'aide alimentaire internationale. |
| Sous-nutrition | Analyser le nombre de personnes en situation de sous-nutrition selon les pays et les périodes disponibles. |

Ces sources permettent de croiser des informations démographiques et alimentaires pour construire des indicateurs comparables.

## Méthodologie

### 1. Exploration des données

La première étape consiste à importer les fichiers et à examiner leur structure.

Pour chaque jeu de données, j'étudie notamment :
- le nombre de lignes et de colonnes ;
- les types de variables ;
- la présence de valeurs manquantes ;
- les premières observations ;
- les unités utilisées et leur cohérence.

Cette exploration permet de comprendre les données disponibles et d'identifier les transformations nécessaires avant l'analyse.

### 2. Préparation et harmonisation

Les données provenant de plusieurs sources nécessitent des transformations pour pouvoir être exploitées conjointement.

Les traitements comprennent notamment :
- l'harmonisation des unités de population ;
- la conversion des variables en types numériques adaptés ;
- le traitement des valeurs particulières présentes dans les données de sous-nutrition ;
- l'harmonisation des périodes étudiées ;
- le rapprochement des jeux de données à partir des pays et des années.

Une attention particulière est portée aux valeurs exprimant des situations de sous-nutrition inférieures à un seuil, afin de ne pas les confondre avec des données absentes.

### 3. Analyse de la sous-nutrition mondiale

Une partie importante de l'étude porte sur la proportion de la population mondiale en situation de sous-nutrition en 2017.

Le calcul repose sur le rapprochement des données de population et de sous-nutrition, puis sur l'agrégation des résultats à l'échelle mondiale.

**Résultat principal :**
- Nombre de personnes en situation de sous-nutrition : 535,7 millions.
- Proportion de la population mondiale concernée : 7,1 %.

Ces indicateurs permettent de mesurer l'ampleur du phénomène à l'échelle mondiale sur la période étudiée.

### 4. Analyse comparative entre les pays

L'étude comprend également des analyses à l'échelle nationale afin de mettre en évidence les différences entre les situations alimentaires.

Le calcul d'indicateurs rapportés à la population permet de comparer les pays sans se limiter aux seuls effectifs absolus.

Une analyse spécifique de la Thaïlande figure notamment dans le notebook, avec un taux de sous-nutrition calculé à partir des données de population et de sous-nutrition disponibles pour 2017.

### 5. Visualisation cartographique

Pour faciliter l'interprétation des résultats, une carte interactive est réalisée avec Plotly.

Elle représente la proportion de personnes en situation de sous-nutrition par pays en 2017.

Cette visualisation permet :
- de comparer les situations géographiques ;
- de repérer les disparités entre les pays ;
- de consulter les informations associées à chaque pays ;
- de distinguer les valeurs disponibles des données manquantes.

La représentation cartographique complète les indicateurs chiffrés en apportant une lecture géographique des résultats.

## Principaux résultats

### Une problématique mondiale majeure

L'étude estime à 535,7 millions le nombre de personnes en situation de sous-nutrition en 2017, soit 7,1 % de la population mondiale.

Ce résultat met en évidence l'importance de la sous-nutrition à l'échelle internationale.

### Des situations différentes selon les pays

L'analyse par pays permet de dépasser la seule moyenne mondiale et d'étudier les disparités géographiques.

Le recours à des proportions rapportées à la population facilite les comparaisons entre des pays dont les effectifs démographiques sont très différents.

### L'intérêt du croisement des données

Le rapprochement des données démographiques et alimentaires permet de construire des indicateurs plus pertinents que ceux obtenus en étudiant chaque fichier isolément.

Cette approche constitue une étape essentielle pour analyser des problématiques complexes à partir de sources hétérogènes.

## Outils et bibliothèques

| Outil ou bibliothèque | Utilisation |
|---|---|
| Python | Langage utilisé pour l'analyse des données. |
| Jupyter Notebook | Environnement de travail permettant de combiner code, explications et visualisations. |
| Pandas | Importation, exploration, préparation, transformation et rapprochement des données. |
| NumPy | Manipulation de données numériques. |
| Matplotlib | Création de visualisations. |
| Plotly Express | Création de visualisations interactives et de cartes choroplèthes. |
| PyCountry | Exploitation des référentiels de pays et de leurs codes. |
| Country Converter | Harmonisation des noms de pays et conversion des référentiels géographiques. |

## Livrables

### Notebook d'analyse

Le notebook Jupyter contient les différentes étapes de l'étude : importation des données, exploration, préparation, calcul des indicateurs et visualisations.

[Consulter le notebook Jupyter](./Capell_Gabriel_1_notebook_012026.ipynb)

### Présentation des résultats

La présentation PowerPoint constitue un support de synthèse des travaux réalisés et des résultats de l'étude.

[Consulter la présentation PowerPoint](./Capell_Gabriel_3_presentation_122025.pptx)

## Compétences mobilisées

| Domaine | Compétences |
|---|---|
| Programmation | Utilisation de Python dans un environnement Jupyter. |
| Manipulation de données | Exploration et transformation de données avec Pandas et NumPy. |
| Préparation des données | Harmonisation des unités, des types de variables et des référentiels géographiques. |
| Jointures | Rapprochement de plusieurs sources de données à partir de clés communes. |
| Analyse statistique descriptive | Calcul de proportions et d'indicateurs à partir de données démographiques. |
| Analyse comparative | Étude des différences entre pays. |
| Datavisualisation | Création de graphiques et de cartes interactives. |
| Communication | Présentation structurée des résultats d'une analyse. |

## Conclusion

Ce projet m'a permis de mettre en pratique une démarche d'analyse de données appliquée à une problématique de santé publique.

En combinant plusieurs sources de données, j'ai travaillé sur leur préparation, leur harmonisation et leur rapprochement afin de calculer des indicateurs et d'étudier les disparités entre les pays.

La réalisation de visualisations, notamment cartographiques, m'a également permis de travailler sur la restitution des résultats et leur lisibilité.

Ce projet illustre plusieurs dimensions du métier de Data Analyst : la préparation des données, l'analyse quantitative, la visualisation et la communication des résultats.

---

**Domaine :** santé publique et sécurité alimentaire  
**Langage :** Python  
**Environnement :** Jupyter Notebook  
**Type de projet :** formation Data Analyst  
**Dépôt GitHub :** [gbcpl/projet4data](https://github.com/gbcpl/projet4data)
