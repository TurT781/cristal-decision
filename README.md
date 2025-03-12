# Test Technique Cristal-Decision

## Présentation du projet

Ce projet a été réalisé dans le cadre d'un test technique pour l'entreprise Cristal-Decision, pour une candidature en alternance de 3ème année à Epitech. L'objectif était d'analyser un jeu de données énergétiques avec des relevés effectués toutes les 10 minutes du 1/4/2020 au 1/3/2022.

## Fonctionnalités

Le programme développé permet de :

- Charger et prétraiter des données à partir d'un fichier CSV
- Segmenter les données selon différentes plages horaires et jours de la semaine :
  - **Tiroir 1** : Lundi à Vendredi de 08h00 à 20h00
  - **Tiroir 2** : Samedi de 08h00 à 20h00
  - **Tiroir 3** : Le reste des données (dimanches et périodes nocturnes)
- Visualiser les données sous forme de graphiques à barres pour une analyse comparative

## Technologies utilisées

- **Python** (environnement Anaconda)
- **Pandas** pour le traitement et la manipulation des données
- **Plotly** pour la création de visualisations interactives

## Structure du code

Le code réalise les opérations suivantes :

1. Chargement des données depuis un fichier CSV
2. Conversion et formatage des dates et heures
3. Segmentation des données en trois "tiroirs" selon les critères temporels
4. Calcul des valeurs en kWh (en tenant compte de l'intervalle de 10 minutes)
5. Création de visualisations distinctes pour chaque segment

## Visualisations

Le projet génère trois visualisations principales :

- 🔴 Un **graphique à barres** pour les jours de semaine (lundi-vendredi) de 8h à 20h
- 🔵 Un **graphique à barres** pour les samedis de 8h à 20h
- 🟢 Un **graphique à barres** pour le reste des données (dimanches et heures nocturnes)

![tiroir1](/results/img/figWeekday.png)
![tiroir2](/results/img/figSaturday.png)
![tiroir3](/results/img/figRemainder.png)


_Les graphiques sont intentionnellement réduit à **7 jours** pour une meilleur lisibilité._

_Cepandant il suffit de **"Autoscale"** pour appercevoir l'entierté du graphique._

## Exécution du script

Pour exécuter le script, assurez-vous d'avoir installé les dépendances nécessaires avec :

```bash
pip install pandas plotly
```

Puis, lancez le script avec le bouton:
**run all**

---

**Auteur** : Flavien Patriarca

**Date** : Mars 2025
