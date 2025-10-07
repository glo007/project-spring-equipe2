#  project-spring-equipe2  
**TP DataOps — Projet d’équipe dans le cadre du module Spring / Scrum**

---

#  Projet DataPulse - Sprint 1 (DataOps)

---

##  Contexte du projet

Le projet **DataPulse** s’inscrit dans une démarche **DataOps**, visant à automatiser et fiabiliser les flux de données d’une organisation.  
L’objectif est de concevoir un pipeline complet permettant :
- L’ingestion de données brutes (CSV ou API),
- Leur transformation et nettoyage automatisé,
- Leur stockage dans une base de données structurée,
- Et leur visualisation via un dashboard simple et moderne.

Ce **Sprint 1** a pour but de **simuler un cycle Scrum complet** appliqué à un projet DataOps, en suivant la méthodologie Agile de bout en bout.

---

##  Objectifs du Sprint 1

- Créer le dépôt GitHub et le projet associé (Kanban).  
- Identifier et décrire les **User Stories (US)** principales.  
- Détaillez les **tâches techniques** à réaliser.  
- Estimer la charge de travail avec des **Story Points (suite de Fibonacci)**.  
- Planifier le sprint et répartir les rôles Scrum.  
- Simuler les **événements agiles** (Daily, Review, Retro).  

---

## Organisation Scrum de l’équipe

| Rôle | Membre | Responsabilités |
|------|---------|----------------|
| **Product Owner (PO)** | Ann-jireh | Définit les priorités du backlog, s’assure que le produit répond aux besoins métier et valide les livrables. |
| **Scrum Master (SM)** | Arcy | Facilite la communication, garantit la méthode Scrum et supervise la progression de l’équipe. |
| **Développeur DataOps** | Gloire | Met en place le pipeline de données complet : ingestion, nettoyage, stockage et visualisation. |

---

##  Organisation GitHub Project

**Nom du projet GitHub :** `Sprint 1 - DataOps`  
**Type :** Kanban board  
**Colonnes :**  
-  To do  
-  In Progress  
-  In Review  
-  Done  

Chaque **issue** correspond à une **User Story (US)**.  
Les **tâches techniques** sont listées dans la description de chaque issue.

---

##  Product Backlog — User Stories (US)

| ID | User Story | Description | Critères d’acceptation | Estimation (SP) |
|----|-------------|--------------|-------------------------|-----------------|
| **US1** | Ingestion automatisée des données | En tant que Développeur DataOps, je veux automatiser la récupération de fichiers CSV pour alimenter la base de données. | Le script doit lire les fichiers CSV depuis un dossier et les insérer automatiquement dans la base PostgreSQL. | 5 |
| **US2** | Nettoyage et transformation des données | En tant que Développeur DataOps, je veux transformer et nettoyer les données pour les rendre exploitables. | Les données nettoyées sont stockées dans une table `clean_data`, sans doublons ni valeurs manquantes critiques. | 3 |
| **US3** | Stockage et structuration | En tant que Développeur DataOps, je veux stocker les données nettoyées dans une base PostgreSQL. | Les données doivent être structurées, interrogeables et sécurisées. | 3 |
| **US4** | Visualisation des données | En tant que Développeur DataOps, je veux afficher les résultats dans un dashboard interactif (Streamlit). | Le dashboard affiche au moins 3 indicateurs clés, avec filtrage dynamique. | 8 |
| **US5** | Supervision du pipeline | En tant que Scrum Master, je veux mettre en place des logs et une supervision pour suivre les exécutions. | Un fichier de logs conserve les statuts et erreurs, et des notifications apparaissent en cas d’échec. | 5 |

---

##  Détail des tâches techniques (Sprint Backlog)

| User Story | Tâches | Responsable | Estimation (SP) | Livrable attendu |
|-------------|--------|--------------|------------------|------------------|
| **US1** | Créer le script d’ingestion automatique (`ingestion.py`) | Gloire | 3 | Script Python fonctionnel |
| **US1** | Automatiser l’exécution (scheduler/cron job) | Gloire | 2 | Ingestion automatisée |
| **US2** | Créer le script de nettoyage (`clean_data.py`) | Gloire | 3 | Données nettoyées dans PostgreSQL |
| **US3** | Concevoir le schéma PostgreSQL et configurer la connexion | Gloire | 3 | Base `datapulse_db` connectée |
| **US4** | Créer un dashboard Streamlit (`dashboard.py`) | Gloire | 8 | Dashboard interactif |
| **US5** | Ajouter un système de logs et d’alertes | Arcy | 5 | Fichier de logs et notifications |
| **Scrum** | Maintenir la documentation et le backlog | Ann-jireh | 2 | README et suivi du projet |

---

##  Estimation des Story Points (Fibonacci)

| Complexité | Valeur | Description |
|-------------|--------|-------------|
| Très simple | 1 | Configuration ou tâche mineure |
| Simple | 2 | Petite fonction ou test unitaire |
| Moyenne | 3 | Script Python ou transformation de données |
| Complexe | 5 | Pipeline ou supervision complète |
| Très complexe | 8 | Dashboard complet connecté à la base |

---

##  Planification du Sprint 1

| Sprint | Durée | Objectifs principaux |
|--------|--------|----------------------|
| **Sprint 1** | 1 semaine | Construire un pipeline de données automatisé (ingestion → nettoyage → stockage → visualisation). |

###  Livrables attendus
- Scripts Python fonctionnels (`ingestion.py`, `clean_data.py`)  
- Base PostgreSQL connectée  
- Dashboard Streamlit affichant les indicateurs  
- Système de logs et documentation complète  

---

##  Événements Scrum simulés

| Événement | Objectif | Durée indicative |
|------------|-----------|------------------|
| **Sprint Planning** | Définir les US du sprint et planifier les tâches | 1h |
| **Daily Scrum** | Synchroniser l’équipe et signaler les obstacles | 15 min/jour |
| **Sprint Review** | Présenter les livrables au Product Owner | 30 min |
| **Sprint Retrospective** | Identifier les axes d’amélioration | 30 min |

---

##  Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
|  Ce qui a bien fonctionné | Collaboration fluide et forte autonomie technique. |
|  À améliorer | Gestion du temps sur certaines tâches techniques. |
|  Pour le prochain sprint | Automatiser davantage et ajouter des tests unitaires. |

---

#  Documentation Scrum intégrée

---

## Principe de la méthode Scrum

Scrum repose sur 3 piliers :
- **Transparence** : tout le monde voit l’avancement via le Kanban GitHub.  
- **Inspection** : l’équipe analyse ses résultats à chaque sprint.  
- **Adaptation** : les méthodes sont ajustées à chaque itération pour être plus efficaces.

---

##  Rôles dans l’équipe Scrum

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| **Product Owner (PO)** | Ann-jireh | Gère le backlog produit, fixe les priorités, valide les livrables. |
| **Scrum Master (SM)** | Arcy| Garantit la méthode Scrum, anime les cérémonies et supprime les obstacles. |
| **Développeur DataOps** | Gloire | Développe, teste et automatise le pipeline complet de données. |

---

##  Artefacts Scrum

| Artefact | Description |
|-----------|-------------|
| **Product Backlog** | Liste priorisée des User Stories du projet. |
| **Sprint Backlog** | Ensemble des tâches à réaliser durant le sprint actuel. |
| **Incrément** | Résultat livrable à la fin du sprint : un pipeline de données fonctionnel. |

---

##  Événements Scrum

| Événement | Description | Objectif |
|------------|-------------|-----------|
| **Sprint Planning** | Début du sprint : planification des tâches et objectifs. | Organiser le travail de la semaine. |
| **Daily Scrum** | Courte réunion quotidienne. | Vérifier l’avancement et les blocages. |
| **Sprint Review** | Présentation du résultat. | Valider le travail livré. |
| **Sprint Retrospective** | Analyse du déroulé du sprint. | S’améliorer collectivement. |

---

##  Estimation avec Story Points (suite de Fibonacci)

| Valeur | Niveau de complexité | Exemple |
|---------|----------------------|----------|
| 1 | Très simple | Ajustement mineur |
| 2 | Simple | Ajout de fonction |
| 3 | Moyenne | Script de nettoyage |
| 5 | Complexe | Pipeline complet |
| 8 | Très complexe | Dashboard complet |

---

##  Outils utilisés

| Outil | Rôle dans le projet |
|-------|----------------------|
| **GitHub Projects** | Gestion du backlog et suivi Kanban |
| **Python / Pandas** | Traitement et transformation des données |
| **PostgreSQL** | Stockage des données |
| **Streamlit** | Dashboard de visualisation |
| **Logging (Python)** | Supervision du pipeline |
| **Markdown Docs** | Documentation du sprint |

---

##  Bilan Scrum global

| Points forts | Axes d’amélioration |
|---------------|--------------------|
| Communication claire et cohésion d’équipe | Approfondir la supervision automatique |
| Répartition équilibrée des rôles | Gérer le temps sur les tâches complexes |
| Bonne maîtrise technique de Python et GitHub | Ajouter des tests automatisés |

---

## Objectif final

À la fin du **Sprint 1**, l’équipe DataPulse aura :
- Un **pipeline automatisé complet** (ingestion → nettoyage → stockage → dashboard),  
- Une **documentation claire et collaborative**,  
- Et une **mise en œuvre complète de la méthode Scrum / DataOps**.

---

## Références

- [Guide Scrum (Scrum.org)](https://www.scrum.org/resources/scrum-guide)  
- [ GitHub Projects (Kanban)](https://docs.github.com/fr/issues/planning-and-tracking-with-projects)  
- [Python Logging](https://docs.python.org/3/library/logging.html)  
- [Streamlit Documentation](https://docs.streamlit.io/)

---

>  *“Inspecter, adapter et livrer de la valeur — même dans la donnée.”*  
> — Équipe 2 : **Arcy**, **Ann-Jireh**, **Gloire**
