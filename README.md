# 📚 Book Sales & Ratings — Exploratory Data Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=for-the-badge)

**Une analyse exploratoire complète du marché du livre — ventes, évaluations et tendances éditoriales.**

</div>

---

## 🗂️ Table des matières

- [Aperçu du projet](#-aperçu-du-projet)
- [Dataset](#-dataset)
- [Structure du projet](#-structure-du-projet)
- [Visualisations clés](#-visualisations-clés)
- [Principaux insights](#-principaux-insights)
- [Installation & Utilisation](#-installation--utilisation)
- [Stack technique](#-stack-technique)
- [Auteur](#-auteur)

---

## 🔍 Aperçu du projet

Ce projet est une **analyse exploratoire de données (EDA)** appliquée à un dataset de ventes de livres. L'objectif est de comprendre les dynamiques du marché éditorial à travers trois axes principaux :

| Axe | Description |
|-----|-------------|
| 📈 **Analyse de marché** | Identifier les genres, auteurs et périodes les plus performants commercialement |
| 🖊️ **Performance des auteurs** | Évaluer l'impact de la réputation d'un auteur sur ses ventes et ses notes |
| 🔎 **Analyse des tendances** | Détecter l'évolution des préférences de lecture et des habitudes éditoriales |

---

## 📦 Dataset

> **Source :** [Kaggle — Books Sales and Ratings](https://www.kaggle.com/)

Le dataset contient des informations détaillées sur des milliers de livres :

| Colonne | Description |
|---------|-------------|
| `Publishing Year` | Année de publication |
| `Book Name` | Titre du livre |
| `Author` | Nom de l'auteur |
| `Author_Rating` | Niveau de l'auteur (Novice / Intermediate / Famous / Excellent) |
| `Book_average_rating` | Note moyenne attribuée par les lecteurs |
| `Book_ratings_count` | Nombre d'évaluations reçues |
| `genre` | Genre littéraire (fiction, nonfiction, children, genre fiction) |
| `gross sales` | Ventes brutes totales |
| `publisher revenue` | Revenus de l'éditeur |
| `sale price` | Prix de vente |
| `sales rank` | Classement des ventes |
| `units sold` | Nombre d'exemplaires vendus |

---

## 🗃️ Structure du projet

```
📁 book-sales-eda/
│
├── 📓 Book_Sale_EDA.ipynb        # Notebook principal — EDA complet
│
├── 📁 visualisations/
│   ├── distribution_notes_livres.png
│   ├── heatmap_correlation.png
│   ├── livres_par_annee.png
│   ├── nombre_avis_vs_note.png
│   ├── note_auteur_vs_note_livre.png
│   ├── notes_par_genre.png
│   ├── prix_vs_unites_vendues.png
│   ├── revenus_par_genre.png
│   └── top_auteurs_unites_vendues.png
│
└── 📄 README.md
```

---

## 📊 Visualisations clés

<table>
  <tr>
    <td align="center"><b>Distribution des notes</b><br><img src="visualisations/distribution_notes_livres.png" width="380"/></td>
    <td align="center"><b>Heatmap de corrélation</b><br><img src="visualisations/heatmap_correlation.png" width="380"/></td>
  </tr>
  <tr>
    <td align="center"><b>Publications par année</b><br><img src="visualisations/livres_par_annee.png" width="380"/></td>
    <td align="center"><b>Revenus par genre</b><br><img src="visualisations/revenus_par_genre.png" width="380"/></td>
  </tr>
  <tr>
    <td align="center"><b>Top 10 auteurs</b><br><img src="visualisations/top_auteurs_unites_vendues.png" width="380"/></td>
    <td align="center"><b>Prix vs Unités vendues</b><br><img src="visualisations/prix_vs_unites_vendues.png" width="380"/></td>
  </tr>
</table>

---

## 💡 Principaux insights

### 🏆 La genre fiction domine le marché
La genre fiction génère à elle seule plus de **1.6 million de ventes brutes**, soit plus de 7x le chiffre de la nonfiction (2ème). Les stratégies de stock et de marketing doivent prioritairement cibler ce segment.

### 💰 Prix bas = volumes élevés
Les livres vendus à **moins de 10€** concentrent la quasi-totalité des gros volumes de vente (30 000–60 000 unités). Au-delà de 15€, les ventes chutent drastiquement. Une politique tarifaire accessible est un levier de volume déterminant.

### ⭐ La note moyenne ne prédit pas les ventes
Malgré une corrélation quasi nulle entre `Book_average_rating` et `units sold`, les livres sont massivement concentrés autour de **4.0/5**. La visibilité et la réputation de l'auteur sont des facteurs plus déterminants que la seule qualité perçue.

### 📖 Les séries fidélisent et vendent
Le top 10 des auteurs est dominé par des créateurs de **longues séries** (Stephen King, Janet Evanovich, Jim Butcher, Robert Jordan). La fidélisation via les séries est un avantage concurrentiel structurel dans l'industrie du livre.

### 📅 Explosion de la production depuis les années 2000
Le nombre de publications annuelles a crû de façon **exponentielle** à partir des années 2000, avec un pic autour de 2010-2015. Cette intensification de la concurrence rend les décisions data-driven plus nécessaires que jamais pour les éditeurs.

---

## ⚙️ Installation & Utilisation

### 1. Cloner le dépôt

```bash
git clone https://github.com/votre-username/book-sales-eda.git
cd book-sales-eda
```

### 2. Créer un environnement virtuel (recommandé)

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
```

### 3. Installer les dépendances

```bash
pip install -r requirements.txt
```

> **Dépendances principales :** `pandas`, `numpy`, `matplotlib`, `seaborn`, `jupyter`

### 4. Lancer le notebook

```bash
jupyter notebook Book_Sale_EDA.ipynb
```

---

## 🛠️ Stack technique

| Outil | Usage |
|-------|-------|
| **Python 3.12** | Langage principal |
| **Pandas** | Manipulation et nettoyage des données |
| **NumPy** | Calculs numériques |
| **Matplotlib** | Visualisations statiques |
| **Seaborn** | Visualisations statistiques avancées |
| **Jupyter Notebook** | Environnement d'analyse interactif |

---

## 👤 Auteur

<div align="center">

**Projet réalisé dans le cadre d'un EDA académique complet**

[![GitHub](https://img.shields.io/badge/GitHub-Profil-181717?style=for-the-badge&logo=github)](https://github.com/votre-username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profil-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/votre-profil)

*N'hésitez pas à ⭐ le repo si ce projet vous a été utile !*

</div>

---

<div align="center">
<sub>📚 Book Sales & Ratings EDA — Analyse exploratoire du marché du livre</sub>
</div>
