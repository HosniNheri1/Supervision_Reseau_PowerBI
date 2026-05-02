# 📡 Supervision réseau mobile 2G/3G/4G/5G – Dashboard Power BI

## 🎯 Objectif

Ce projet propose un **dashboard de supervision unifié** pour les réseaux mobiles 2G, 3G, 4G et 5G, construit à partir de **données officielles ARCEP** et alimenté par un **flux simulé en quasi temps réel**.

## 🧰 Stack technique

| Outil | Rôle |
|-------|------|
| **Python (pandas, numpy)** | Chargement, nettoyage, fusion des fichiers CSV ARCEP. Simulation d’un flux de données (rafraîchissement toutes les 30 secondes). |
| **Power BI Desktop** | Visualisation interactive : jauges, courbes, slicers, tableau d’alertes, mesures DAX. |
| **Données ARCEP** | Fichiers `sites`, `mesures QoS` et `crowdsourcing Ookla` – couvrant 2G/3G/4G/5G. |

## 📊 Fonctionnalités principales

- ✅ **Supervision multi‑générations** : bascule dynamique entre 2G, 3G, 4G, 5G.
- ✅ **Comparaison opérateurs** : Orange, Free, Bouygues, SFR.
- ✅ **Alertes visuelles** : mise en forme conditionnelle des seuils de débit.
- ✅ **KPIs clés** : débit descendant (Mbps), latence (ms), taux d’alerte.
- ✅ **Simulation temps réel** : ajout d’une ligne toutes les 30 secondes → actualisation Power BI pour démonstration.

## 📁 Structure du dépôt
