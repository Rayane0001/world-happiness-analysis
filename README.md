# Analyse du Bonheur Mondial

## Auteurs

- **Zaoui Gibril**
- **Rousseau Rayane**

## Clonage du Projet

Vous pouvez cloner ce projet directement depuis GitHub :

```bash
git clone https://github.com/Rayane0001/world-happiness-analysis
```

## Description

Ce projet explore les facteurs qui influencent le bonheur à travers le monde. En utilisant Python et plusieurs jeux de données (principalement de Kaggle), nous analysons comment des éléments comme l’économie, la société, la santé, la gouvernance et l’environnement sont liés au bien-être des populations.  
Les analyses et visualisations sont présentées dans le notebook Jupyter `happiness_analysis.ipynb`.

## Questions Analytiques

Le projet explore les 15 grandes questions suivantes :

1. **Impact Relatif des Facteurs sur le Bonheur**  
2. **Pays "Hors Normes" Économiques**  
3. **Disparités Régionales du Bonheur**  
4. **Liberté et Bien-être selon le Contexte**  
5. **Confiance Gouvernementale et Corruption**  
6. **Générosité et Résilience Économique**  
7. **Analyse du Résidu Inexpliqué (Dystopia Residual)**  
8. **Soutien Social et Bien-être par Régions**  
9. **Interaction entre Liberté et Corruption sur le Bonheur**  
10. **Évolution Temporelle du Bonheur et de ses Facteurs**  
11. **Bonheur Évaluatif vs. Affects Émotionnels par Région**  
12. **Inégalités de Genre, Développement (HDI) et Bonheur**  
13. **Santé Spécifique et Bonheur (Contrôlé par le PIB)**  
14. **Développement Durable - Bonheur, Développement et Empreinte Écologique**  
15. **Profils de Gouvernance - Interaction Liberté Objective et Corruption**  

### Conclusion Générale  
Une **carte du bonheur** a été réalisée pour visualiser les pays où il fait le mieux vivre, et nous concluons en prenant en compte l'ensemble des critères étudiés.

## Structure du Projet

```
.
├── happiness_analysis.ipynb  # Notebook Jupyter avec les analyses
├── CSVs/                     # Données utilisées (Source principale: Kaggle)
│   ├── civil_liberties_score_fh_new.csv
│   ├── CPI2023_global_results_trends.csv
│   ├── hdr_general.csv
│   ├── world_happiness_report_2024.csv
│   └── world_population_and_health.csv
├── .gitignore
└── README.md
```

## Données (`CSVs/`)

Ce projet utilise 5 jeux de données principaux, téléchargés depuis [Kaggle](https://www.kaggle.com/) (les sources exactes peuvent varier, ces fichiers combinent des données du World Happiness Report, PNUD, Banque Mondiale, Freedom House, Transparency International) :

1. **`world_happiness_report_2024.csv`** : Données centrales avec scores de bonheur (Life Ladder) et les 6 facteurs clés (PIB/hab, soutien social, espérance de vie, liberté, générosité, corruption), affects.
2. **`hdr_general.csv`** : Indicateurs de Développement Humain (IDH), inégalités de genre, éducation, indicateurs environnementaux (CO2).
3. **`CPI2023_global_results_trends.csv`** : Indice de Perception de la Corruption 2023 et classification régionale.
4. **`civil_liberties_score_fh_new.csv`** : Scores de libertés civiles (Freedom House).
5. **`world_population_and_health.csv`** : Population et indicateurs de santé spécifiques (mortalité infantile, sous-nutrition).

## Prérequis et Installation

**Prérequis :**  
- Python 3.x  
- Bibliothèques Python listées ci-dessous.  

Il est recommandé d’utiliser un environnement virtuel. Pour installer les dépendances, exécutez :

```bash
pip install pandas numpy matplotlib seaborn statsmodels plotly openpyxl xlrd
```

## Bibliothèques Utilisées

- **pandas** : Manipulation des données. Indispensable pour lire les fichiers CSV, nettoyer les données (gérer les valeurs manquantes, filtrer), sélectionner des colonnes, fusionner les différents tableaux (DataFrames) et organiser les informations pour l'analyse.
- **numpy** : Calcul numérique. Utilisé pour les opérations mathématiques efficaces sur les tableaux de données, souvent en arrière-plan de pandas. Nous l'avons aussi utilisé directement pour créer les catégories de profils de gouvernance (`np.select`).
- **matplotlib.pyplot** : Graphiques de base. Sert de fondation pour la plupart des visualisations. Utilisée pour créer les figures, les sous-graphiques, ajouter des titres, des labels, et personnaliser l'apparence des graphiques statiques.
- **seaborn** : Visualisations statistiques avancées. Construit sur matplotlib, seaborn simplifie la création de graphiques statistiques courants et esthétiques comme les nuages de points avec droite de régression (`regplot`, `lmplot`), les heatmaps (pour les corrélations), les diagrammes à barres (`barplot`), les box plots, et les graphiques facettés (pour comparer par catégorie).
- **statsmodels** : Modélisation statistique. Essentiel pour effectuer les analyses de régression linéaire (OLS), y compris les modèles avec termes d'interaction, et pour obtenir des résumés statistiques détaillés (coefficients, p-values, R², etc.) afin de tester nos hypothèses. Utilisé aussi pour les graphiques de régression partielle.
- **plotly.graph_objects** : Graphiques interactifs. Utilisé spécifiquement pour créer la carte mondiale (choroplèthe) interactive qui montre la répartition du bonheur, offrant une alternative à geopandas.

## Utilisation

1. Placez les fichiers CSV dans le sous-dossier `CSVs/`.
2. Ouvrez le notebook `happiness_analysis.ipynb` avec **JupyterLab, Jupyter Notebook, VS Code, PyCharm** ou tout autre IDE compatible.
3. Exécutez les cellules dans l’ordre pour obtenir les analyses, visualisations et interprétations détaillées.

## Résumé des Résultats

Le bonheur ne dépend pas uniquement de l’argent ! Des liens sociaux forts, un sentiment de liberté, une bonne santé, une faible corruption et une certaine égalité sont tout aussi, voire plus, importants.  
Le monde est très inégal face au bonheur, et concilier bien-être élevé et respect de l’environnement reste un défi majeur.  
Les pays qui réussissent le mieux combinent souvent **performance économique, cohésion sociale et bonne gouvernance**.