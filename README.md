# 🏃 Boston Marathon 2024 - Data Visualization

> Projet de visualisation de données réalisé dans le cadre du cours **DataViz** à l'ESILV (2025-2026).

![D3.js](https://img.shields.io/badge/D3.js-v7-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

## 📋 Description

Ce projet analyse les données du **Boston Marathon 2024** à travers deux visualisations interactives développées avec D3.js. L'objectif est d'explorer les origines géographiques des coureurs, leurs stratégies de course et leurs performances.

## 🎯 Visualisations

### 1. Carte Choroplèthe - Origine des Coureurs
Une carte interactive des États-Unis permettant de visualiser :
- **Nombre de coureurs** par état
- **Temps moyen** de finish par état
- **Température moyenne** d'origine des coureurs

### 2. Diagramme Sankey - Stratégies de Course
Un diagramme de flux montrant la relation entre :
- La **stratégie de course** adoptée (Negative/Even/Positive Split)
- Le **temps final** de la course

## 🚀 Démo en ligne

👉 **[Voir le projet](https://matheorie.github.io/marathon-dataviz/)**

## 🛠️ Technologies utilisées

- **D3.js v7** - Bibliothèque de visualisation
- **TopoJSON** - Données géographiques USA
- **d3-sankey** - Plugin pour diagramme Sankey
- **HTML5 / CSS3** - Structure et style
- **GitHub Pages** - Hébergement

## 📁 Structure du projet

```
marathon-dataviz/
├── index.html              # Dashboard principal
├── map-marathon.html       # Visualisation carte
├── sankey-marathon.html    # Visualisation Sankey
├── data/
│   ├── Athletes.csv        # Données des coureurs
│   └── Weather.csv         # Données météo par ZIP
└── README.md               # Documentation
```

## 📊 Données

Les données proviennent de [Kaggle - 2024 Boston Marathon Weather and Splits](https://www.kaggle.com/datasets/runningwithrock/2024-boston-marathon-weather-and-splits) et incluent :

| Fichier | Description |
|---------|-------------|
| `Athletes.csv` | Informations sur chaque coureur (bib, temps, ZIP, etc.) |
| `Weather.csv` | Température moyenne par code postal |

### Variables principales

- `Bib` : Numéro de dossard
- `Finish` : Temps de finish en secondes
- `Zip` : Code postal d'origine
- `Percent Change` : Variation de rythme entre les deux moitiés

## 🏗️ Installation locale

1. **Cloner le repository**
   ```bash
   git clone https://github.com/matheorie/marathon-dataviz.git
   cd marathon-dataviz
   ```

2. **Lancer un serveur local** (nécessaire pour charger les CSV)
   ```bash
   # Avec Python 3
   python -m http.server 8000
   
   # Ou avec Node.js
   npx serve
   ```

3. **Ouvrir dans le navigateur**
   ```
   http://localhost:8000
   ```

## 📈 Insights clés

- **17,209 coureurs** analysés provenant de 50 états
- Le **Massachusetts** est l'état le plus représenté (proximité de Boston)
- La majorité des coureurs adoptent un **positive split** (ralentissement)
- Les coureurs avec un **negative split** obtiennent généralement de meilleurs temps

## 👥 Auteurs

| Nom | Rôle |
|-----|------|
| **Mathéo Judenne** | Développement & Visualisations |
| **Gauthier Le Brun** | Développement & Visualisations |
| **Jaël Ribere** | Développement & Visualisations |
| **Paul Bruneton** | Développement & Visualisations |

---

*Projet réalisé dans le cadre du cours DataViz - ESILV 2025-2026*
