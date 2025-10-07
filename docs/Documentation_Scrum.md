# 📘 Documentation Scrum - Projet DataPulse (Sprint 1)

---

## 🧩 Contexte général

Le projet **DataPulse** a été réalisé dans le cadre du **TP DataOps – Module Spring/Scrum**.  
L’objectif est de simuler un **sprint complet Scrum**, autour d’un projet DataOps dont la mission principale est de concevoir un pipeline de données automatisé permettant :

- l’ingestion de fichiers CSV,
- le nettoyage et la transformation des données,
- leur stockage dans une base PostgreSQL,
- et leur visualisation via un dashboard Streamlit.

Ce sprint illustre l’application des **valeurs Scrum** : collaboration, transparence, inspection et adaptation continue.

---

## 👥 Organisation de l’équipe Scrum

| Rôle                    | Membre    | Responsabilités principales                                                                     |
| ----------------------- | --------- | ----------------------------------------------------------------------------------------------- |
| **Product Owner (PO)**  | Arcy      | Définit les priorités du backlog, veille à la valeur métier et valide les livrables.            |
| **Scrum Master (SM)**   | Ann-Jireh | Facilite la communication, supprime les obstacles et veille au respect de la méthode Scrum.     |
| **Développeur DataOps** | Gloire    | Met en œuvre les scripts Python, la base PostgreSQL, le dashboard et le système de supervision. |

L’équipe travaille de manière collaborative sur GitHub, en suivant un **Kanban agile** via le projet `Sprint 1 - DataOps`.

---

## 🧱 Artefacts Scrum

### 📦 1. Product Backlog

Le **Product Backlog** regroupe toutes les fonctionnalités (User Stories) nécessaires à la réalisation du projet.  
Chaque User Story (US) décrit un besoin utilisateur précis, des critères d’acceptation et des tâches techniques.

Exemples :

- US1 : Ingestion automatisée des données CSV
- US2 : Nettoyage et transformation des données
- US3 : Stockage structuré dans PostgreSQL
- US4 : Visualisation dans un dashboard
- US5 : Supervision du pipeline
- US6 : Documentation et gestion du backlog

---

### 📋 2. Sprint Backlog

Le **Sprint Backlog** contient les User Stories sélectionnées pour ce sprint d’une semaine.  
Elles sont réparties dans le **Kanban GitHub** :

> To do → In progress → In review → Done

---

### 🧩 3. Incrément

L’incrément représente le résultat livré à la fin du sprint :

- Un pipeline fonctionnel de bout en bout (CSV → PostgreSQL → Dashboard),
- Une documentation claire et collaborative,
- Et une supervision automatisée des logs.

---

## 🕒 Événements Scrum simulés

| Événement                | Objectif                                                                   | Durée       | Résultat attendu                        |
| ------------------------ | -------------------------------------------------------------------------- | ----------- | --------------------------------------- |
| **Sprint Planning**      | Planifier les User Stories réalisables pendant le sprint.                  | 1h          | Sprint Backlog validé                   |
| **Daily Scrum**          | Faire le point chaque jour sur l’avancement et les obstacles.              | 15 min/jour | Suivi d’équipe et mise à jour du Kanban |
| **Sprint Review**        | Présenter les livrables au Product Owner et recueillir des retours.        | 30 min      | Validation ou ajustements du produit    |
| **Sprint Retrospective** | Identifier les points forts et axes d’amélioration pour le sprint suivant. | 30 min      | Plan d’amélioration continue            |

---

## 🧮 Estimation avec Story Points

L’équipe a utilisé la **suite de Fibonacci (1, 2, 3, 5, 8)** pour estimer la charge de travail de chaque tâche selon sa complexité.

| Valeur | Niveau de complexité | Exemple                          |
| ------ | -------------------- | -------------------------------- |
| 1      | Très simple          | Ajustement mineur ou mise à jour |
| 2      | Simple               | Script de test ou configuration  |
| 3      | Moyenne              | Script Python autonome           |
| 5      | Complexe             | Pipeline complet ou supervision  |
| 8      | Très complexe        | Dashboard connecté et interactif |

---

## 🗓️ Planification du Sprint 1

| User Story                            | Responsable | Estimation | Livrable attendu                  |
| ------------------------------------- | ----------- | ---------- | --------------------------------- |
| **US1** - Ingestion automatisée       | Gloire      | 5          | Script `ingestion.py`             |
| **US2** - Nettoyage et transformation | Gloire      | 3          | Script `clean_data.py`            |
| **US3** - Stockage structuré          | Gloire      | 3          | Base PostgreSQL `datapulse_db`    |
| **US4** - Visualisation               | Gloire      | 8          | Dashboard Streamlit               |
| **US5** - Supervision                 | Ann-Jireh   | 5          | Système de logs et alertes        |
| **US6** - Documentation / Backlog     | Arcy        | 3          | README complet et suivi de projet |

---

## 📊 Outils utilisés

| Outil                        | Utilisation                               |
| ---------------------------- | ----------------------------------------- |
| **GitHub Projects (Kanban)** | Suivi du sprint et répartition des tâches |
| **Issues GitHub**            | Création et suivi des User Stories        |
| **Python + Pandas**          | Ingestion et traitement des données       |
| **PostgreSQL**               | Stockage et structuration                 |
| **Streamlit**                | Création du dashboard                     |
| **Logging (Python)**         | Supervision et rapports d’erreurs         |
| **Markdown Docs**            | Documentation projet et Scrum             |

---

## 🔁 Cycle de vie du Sprint

Chaque itération se conclut par une **version livrable et documentée** du pipeline DataOps.

---

## 📈 Bilan du Sprint 1

| Question                            | Réponse                                                                  |
| ----------------------------------- | ------------------------------------------------------------------------ |
| ✅ Ce qui a bien fonctionné         | Bonne coordination d’équipe et respect des rôles Scrum.                  |
| ⚠️ Ce qui aurait pu mieux se passer | Gestion du temps sur certaines tâches techniques.                        |
| 🚀 Ce qu’on va améliorer            | Automatiser davantage et ajouter des tests unitaires pour chaque script. |

---

## 🎯 Objectif final

À la fin du Sprint 1, l’équipe **DataPulse (Équipe 2)** doit :

- Avoir un pipeline DataOps complet, automatisé et documenté,
- Fournir un dashboard fonctionnel connecté à la base PostgreSQL,
- Présenter une organisation Scrum fluide et bien structurée.

---

## 📚 Références

- [Guide Scrum - Scrum.org](https://www.scrum.org/resources/scrum-guide)
- [GitHub Projects (Kanban)](https://docs.github.com/fr/issues/planning-and-tracking-with-projects)
- [Python Logging Documentation](https://docs.python.org/3/library/logging.html)
- [Streamlit Documentation](https://docs.streamlit.io/)
