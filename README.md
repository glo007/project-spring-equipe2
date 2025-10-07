# 🧱 project-spring-equipe2  
**TP DataOps — Projet d’équipe dans le cadre du module Spring / Scrum**

---

# 🚀 Projet DataPulse - Sprint 1 (DataOps)

---

## 🧩 Contexte du projet

Le projet **DataPulse** s’inscrit dans une démarche **DataOps**, visant à automatiser et fiabiliser les flux de données d’une organisation.  
L’objectif est de concevoir un pipeline complet permettant :
- L’ingestion de données brutes (CSV ou API),
- Leur transformation et nettoyage automatisé,
- Leur stockage dans une base de données structurée,
- Et leur visualisation via un dashboard simple et moderne.

Ce sprint a pour but de **simuler un cycle Scrum complet** appliqué à un projet DataOps.

---

## 🎯 Objectifs du Sprint 1

- Créer le dépôt GitHub et le projet associé (Kanban).  
- Identifier et décrire les **User Stories (US)** principales.  
- Détaillez les **tâches techniques** à réaliser.  
- Estimer la charge de travail avec des **Story Points (suite de Fibonacci)**.  
- Planifier le sprint et répartir les rôles Scrum.  
- Simuler les **événements agiles** (Daily, Review, Retro).  

---

## 👥 Organisation Scrum de l’équipe

| Rôle | Membre | Responsabilités |
|------|---------|----------------|
| **Product Owner (PO)** | Arcy | Définit les priorités du backlog, s’assure que le produit répond aux besoins métier. |
| **Scrum Master (SM)** | Jireh | Facilite la communication, veille au respect de la méthode agile. |
| **Data Engineer** | Gloire | Développe les pipelines de données et automatise les flux d’ingestion. |
| **Data Analyst** | Mohammed | Nettoie et analyse les données, conçoit le dashboard de visualisation. |
| **DevOps Engineer** | Mhammed | Gère la supervision, les logs et la fiabilité des traitements automatisés. |

---

## 🗂️ Organisation GitHub Project

**Nom du projet GitHub :** `Sprint 1 - DataOps`  
**Type :** Kanban board  
**Colonnes :**  
- 📋 Backlog (To do)  
- ⚙️ In Progress  
- 🔍 In Review  
- ✅ Done  

Chaque **issue** représente une **User Story (US)**.  
Les **tâches techniques** sont listées dans la description de chaque issue.

---

## 📋 Product Backlog — User Stories (US)

| ID | User Story | Description | Critères d’acceptation | Estimation (SP) |
|----|-------------|--------------|-------------------------|-----------------|
| **US1** | Ingestion automatisée des données | En tant que Data Engineer, je veux automatiser la récupération de fichiers CSV pour alimenter la base de données. | Le pipeline doit lire automatiquement les fichiers d’un dossier et les insérer en base. | 5 |
| **US2** | Nettoyage et transformation des données | En tant que Data Analyst, je veux transformer les données pour les rendre exploitables (valeurs manquantes, formatage, doublons). | Les données nettoyées doivent être stockées dans une table `clean_data`. | 3 |
| **US3** | Stockage structuré | En tant que DevOps Engineer, je veux stocker les données transformées dans une base PostgreSQL. | Les données doivent être accessibles via SQL. | 3 |
| **US4** | Visualisation des données | En tant que Data Analyst, je veux afficher les résultats dans un dashboard (via Streamlit). | Le dashboard doit afficher au moins trois indicateurs principaux. | 8 |
| **US5** | Supervision du pipeline | En tant que DevOps Engineer, je veux mettre en place des logs et alertes d’erreur. | Le système doit notifier en cas d’échec et conserver un journal d’exécution. | 5 |

---

## 🧩 Détail des tâches techniques (Sprint Backlog)

| User Story | Tâche | Responsable | Estimation (SP) | Livrable attendu |
|-------------|-------|--------------|------------------|------------------|
| US1 | Créer le script d’ingestion (Python) | Gloire | 3 | Script d’import automatique depuis un dossier CSV |
| US1 | Automatiser l’exécution via cron job ou scheduler | Mhammed | 2 | Ingestion automatisée |
| US2 | Créer le script de nettoyage (Pandas) | Mohammed | 3 | Données nettoyées et formatées |
| US3 | Concevoir le schéma PostgreSQL | Gloire | 3 | Base PostgreSQL fonctionnelle |
| US3 | Connecter Python à PostgreSQL (SQLAlchemy) | Mhammed | 2 | Connexion validée |
| US4 | Créer un dashboard Streamlit | Mohammed | 5 | Dashboard affichant les KPIs |
| US5 | Ajouter un système de logs | Mhammed | 3 | Fichier de logs et console |
| US5 | Mettre en place une alerte par mail/terminal | Jireh | 2 | Notification d’erreur automatisée |

---

## 🧮 Estimation des Story Points (Fibonacci)

| Complexité | Valeur | Description |
|-------------|--------|-------------|
| Très simple | 1 | Configuration, correctif mineur |
| Simple | 2 | Script ou fonction courte |
| Moyenne | 3 | Script autonome avec dépendances |
| Complexe | 5 | Pipeline complet ou dashboard |
| Très complexe | 8 | Intégration multiple avec dashboard et DB |

---

## 🗓️ Planification du Sprint 1

| Sprint | Durée | Objectifs principaux |
|--------|--------|----------------------|
| Sprint 1 | 1 semaine | Mettre en place l’ingestion, le nettoyage et le stockage initial. |

### 🎯 Livrables
- Scripts Python fonctionnels  
- Base PostgreSQL connectée  
- Dashboard Streamlit minimal  
- Documentation complète du sprint  

---

## 🌀 Événements Scrum simulés

| Événement | Objectif | Durée indicative |
|------------|-----------|------------------|
| **Sprint Planning** | Définir les US et tâches réalisables du sprint | 1h |
| **Daily Scrum** | Synchroniser les membres (15 min/jour) | 15 min |
| **Sprint Review** | Présenter les livrables au PO | 30 min |
| **Sprint Retrospective** | Identifier les axes d’amélioration | 30 min |

---

## 📈 Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
| ✅ Ce qui a bien fonctionné | Collaboration active et communication claire. |
| ⚠️ À améliorer | Estimation plus réaliste des tâches techniques. |
| 🚀 Pour le prochain sprint | Intégrer les tests automatiques et un monitoring avancé. |

---

# 📘 Documentation Scrum intégrée

---

## 🧩 Contexte Scrum

Le projet **DataPulse** applique la méthode **Scrum** afin d’améliorer la qualité du travail d’équipe et de livrer de la valeur à chaque itération.  
L’équipe se base sur trois piliers :  
👉 **Transparence**, **Inspection**, **Adaptation**.

---

## 👥 Rôles Scrum

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| **Product Owner (PO)** | Arcy | Priorise le backlog, définit les objectifs du sprint et valide les livrables. |
| **Scrum Master (SM)** | Jireh | Facilite la méthode Scrum, élimine les obstacles et anime les réunions agiles. |
| **Développeurs Data** | Gloire, Mohammed, Mhammed | Réalisent les tâches techniques (scripts, pipeline, dashboard, logs). |

---

## 🧱 Artefacts Scrum

### 🧩 Product Backlog  
Contient toutes les User Stories définissant les fonctionnalités à développer.

### 🗂️ Sprint Backlog  
Sous-ensemble du Product Backlog sélectionné pour le Sprint 1.

### 🧩 Incrément  
Résultat livrable à la fin du sprint :  
- Pipeline fonctionnel  
- Base PostgreSQL connectée  
- Dashboard Streamlit  
- Système de supervision automatisé

---

## 🕒 Événements Scrum

| Événement | Objectif | Durée |
|------------|-----------|-------|
| **Sprint Planning** | Définir les objectifs et tâches du sprint | 1h |
| **Daily Scrum** | Synchroniser l’équipe, suivre les avancements | 15 min/jour |
| **Sprint Review** | Présenter les résultats au PO et obtenir un feedback | 30 min |
| **Sprint Retrospective** | Identifier les points à améliorer | 30 min |

---

## 🧮 Estimation (Story Points Fibonacci)

| Valeur | Signification | Exemple |
|---------|---------------|----------|
| 1 | Très simple | Script court |
| 2 | Simple | Fonction d’import ou test |
| 3 | Moyenne | Script de nettoyage |
| 5 | Complexe | Pipeline complet |
| 8 | Très complexe | Dashboard connecté |

---

## 📦 Sprint 1 — Planification détaillée

| User Story | Responsable | Estimation | Livrable attendu |
|-------------|--------------|-------------|------------------|
| US1 | Gloire | 5 | Script d’ingestion automatisé |
| US2 | Mohammed | 3 | Script de nettoyage Pandas |
| US3 | Mhammed | 3 | Base PostgreSQL connectée |
| US4 | Mohammed | 8 | Dashboard Streamlit |
| US5 | Jireh / Mhammed | 5 | Système de logs et alertes |

---

## 📊 Outils utilisés

| Outil | Utilisation |
|-------|--------------|
| **GitHub Projects** | Gestion du backlog et suivi Kanban |
| **Python / Pandas** | Traitement et nettoyage des données |
| **PostgreSQL** | Stockage structuré |
| **Streamlit** | Dashboard de visualisation |
| **Logging Python** | Supervision du pipeline |
| **Markdown Docs** | Documentation du sprint |

---

## 🔁 Cycle Scrum

