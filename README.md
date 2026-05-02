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
   git clone https://github.com/HosniNheri1/Supervision_Reseau_PowerBI.git
Ouvrir le projet Power BI
Double‑cliquer sur Graphe-PowerBI.pbip (Power BI Desktop requis).

Lancer le script Python (pour la simulation live)

bash
python supervision_simulator.py
Actualiser le dashboard dans Power BI (bouton Actualiser).
👤 Auteur
Hosni Nheri – GitHub
Projet réalisé dans le cadre du module Réseaux Mobiles sous l’encadrement de Madame Imen Sfaihi.

🙏 Remerciements
Données fournies par l’ARCEP (data.arcep.fr) – licence Open Data.

📄 Licence
Ce projet est distribué sous la licence MIT.
Vous pouvez librement utiliser, modifier et distribuer ce code à des fins personnelles ou commerciales, sous réserve de conserver la mention de l’auteur original.

text
MIT License

Copyright (c) 2025 Hosni Nheri

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

⭐ Un dashboard simple, open source, et entièrement basé sur des données publiques.

📸 Aperçu du dashboard :https://github.com/HosniNheri1/Supervision_Reseau_PowerBI/blob/main/dashboard.png
