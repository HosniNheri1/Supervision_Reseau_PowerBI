markdown
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
.
├── Graphe-PowerBI.Report/ # Modèle Power BI (rapport)
├── Graphe-PowerBI.SemanticModel/ # Modèle sémantique (mesures DAX)
├── .gitignore # Ignore les fichiers cache Power BI
├── Graphe-PowerBI.pbip # Fichier projet (à ouvrir avec Power BI Desktop)
└── README.md

text

## 🚀 Utilisation

1. **Cloner le dépôt**  
   ```bash
   git clone https://github.com/nom-utilisateur/nom-repo.git
Ouvrir le projet Power BI
Double‑cliquer sur Graphe-PowerBI.pbip (Power BI Desktop requis).

Lancer le script Python (pour la simulation live)

bash
python supervision_simulator.py
Actualiser le dashboard dans Power BI (bouton Actualiser).

📌 Pour aller plus loin
Remplacer la simulation Python par une vraie ingestion en continu (API, WebSocket, Kafka).

Publier le rapport sur Power BI Service avec actualisation automatique.

Ajouter des alertes par e‑mail via Power Automate.

🙏 Remerciements
Projet réalisé dans le cadre du module Réseaux Mobiles de Madame Imen Sfaihi – données fournies par l’ARCEP (data.arcep.fr).
⭐ Un dashboard simple, open source, et entièrement basé sur des données publiques.

text

Tu peux aussi **rajouter une capture d’écran** de ton dashboard en enregistrant une image dans le dépôt (ex: `dashboard.png`) puis en l’affichant avec `![Dashboard](./dashboard.png)`.
