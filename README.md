- Analyse et Classement de Données d'Animes

Ce projet propose une analyse approfondie d'un jeu de données d'animes, incluant le nettoyage des données, le calcul de métriques de performance personnalisées et la visualisation des tendances clés. L'objectif est d'évaluer la qualité globale des séries tout en tenant compte de leur régularité entre les meilleurs et les pires épisodes.

- Table des Matières
•Description du Projet
•Fonctionnalités Clés
•Structure du Projet
•Installation
•Utilisation
•Étapes Essentielles
•Technologies Utilisées

- Description du Projet
Le projet utilise un fichier source animes.csv contenant des informations détaillées telles que les studios, les notes globales, et les notes spécifiques des épisodes. À travers un workflow de science de données classique, le notebook transforme ces données brutes en insights exploitables, permettant notamment d'identifier les animes les plus "équilibrés" via un Score Métier pondéré.

- Fonctionnalités Clés
•Nettoyage Automatisé : Conversion des types de données, gestion des valeurs manquantes et filtrage des entrées incomplètes.
•Ingénierie de Caractéristiques (Feature Engineering) :
•Régularité : Calculée en fonction de l'écart entre le meilleur et le pire épisode.
•Score Métier : Une note finale pondérée (70% Note Globale, 30% Régularité).
•Analyse Statistique : Résumés descriptifs des tendances de notation et de production.
•Visualisations de Données : Graphiques illustrant la provenance des œuvres (Manga, Light Novel, Original, etc.) et les distributions de notes.

- Structure du Projet

Plain Text
.
├── Notebook.ipynb        # Le notebook principal contenant l'analyse
├── animes.csv            # Données brutes (entrée)
├── animes_propre.csv     # Données nettoyées (généré par le notebook)
├── graphique_sources.png # Visualisation des sources (généré)
└── README.md             # Documentation du projet


- Installation

Prérequis
•Python 3.8 ou supérieur
•Un environnement Jupyter (JupyterLab, Jupyter Notebook ou VS Code)

- Dépendances
Installez les bibliothèques nécessaires via pip : pip install pandas matplotlib plotly ipython


- Utilisation
1. Placez votre fichier animes.csv dans le même répertoire que le notebook.
2. Ouvrez Notebook.ipynb dans votre environnement Jupyter.
3. Exécutez toutes les cellules pour reproduire l'analyse.
4. Consultez le fichier animes_propre.csv généré pour les données traitées.

- Étapes Essentielles
1. Chargement: Importation des bibliothèques et lecture du fichier CSV initial.
2. Nettoyage: Conversion des notes en formats numériques et suppression des lignes sans score global.
3. Analyse: Calcul de l'écart de notes et création du score de régularité.
4. Scoring: Application de la formule du "Score Métier" pour classer les animes.
5. Visualisation: Génération de graphiques (Top 5 des sources, etc.) pour l'interprétation visuelle.

- Technologies Utilisées
•Pandas : Manipulation et analyse de données.
•Matplotlib : Création de graphiques statiques.
•Plotly : Visualisations interactives.
•Jupyter : Environnement de développement interactif.