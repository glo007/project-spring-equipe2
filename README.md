# project-spring-equipe2
TP DataOps, Projet d’équipe dans le cadre du module Spring / Scrum
# 🚀 Projet DataPulse - Sprint 1 (DataOps)

## 🧩 Contexte du projet

Le projet **DataPulse** s’inscrit dans une démarche **DataOps**, visant à automatiser et fiabiliser les flux de données d’une organisation.  
L’objectif est de concevoir un pipeline complet permettant :
- L’ingestion de données brutes (CSV ou API),
- Leur transformation et nettoyage automatisé,
- Leur stockage dans une base de données structurée,
- Et leur visualisation via un dashboard simple (tableau ou graphique).

Ce sprint a pour but de simuler un cycle **Scrum complet** appliqué à un projet DataOps.

---

## 🎯 Objectifs du Sprint 1

- Créer le dépôt GitHub avec gestion des issues et backlog.  
- Identifier et décrire les **User Stories (US)** principales.  
- Détaillez les **tâches techniques** à réaliser.  
- Estimer la charge de travail avec des **Story Points (Fibonacci)**.  
- Planifier le sprint et répartir les rôles.

---

## 👥 Organisation Scrum de l’équipe

| Rôle | Membre | Responsabilités |
|------|---------|----------------|
| **Product Owner** | Arcy | Définit les priorités du backlog, veille à la valeur métier. |
| **Scrum Master** | Ann-Jireh | Garant de la méthode agile, facilite la communication. |
| **Data Engineer** | Bryan | Met en place les pipelines et transformations de données. |
| **Data Analyst** | Mohammed | Analyse les données et conçoit le tableau de bord final. |
| **DevOps Engineer** | Mhammed | Automatise le déploiement et la supervision des flux. |

---

## 🗂️ Organisation GitHub Project

**Nom du projet GitHub :** `Sprint 1 - DataOps`  
**Type :** Kanban board  
**Colonnes :**  
- 📋 Backlog (To do)  
- ⚙️ In Progress  
- 🔍 In Review  
- ✅ Done  

Chaque **issue** correspond à une **User Story (US)**.  
Les **tâches techniques** seront listées dans la description de chaque issue.

---

## 📋 Product Backlog — User Stories (US)

| ID | User Story | Description | Critères d’acceptation | Estimation (SP) |
|----|-------------|--------------|-------------------------|-----------------|
| **US1** | Ingestion automatisée des données | En tant que Data Engineer, je veux automatiser la récupération de fichiers CSV pour alimenter la base de données. | Le pipeline doit pouvoir lire automatiquement les fichiers d’un dossier et les insérer en base. | 5 |
| **US2** | Nettoyage et transformation des données | En tant que Data Analyst, je veux transformer les données pour les rendre exploitables (valeurs manquantes, formatage, etc.). | Les données nettoyées doivent être stockées dans une table "clean_data". | 3 |
| **US3** | Stockage structuré | En tant que DevOps Engineer, je veux stocker les données transformées dans une base PostgreSQL. | Les données doivent être accessibles via SQL. | 3 |
| **US4** | Visualisation des données | En tant que Data Analyst, je veux afficher les résultats dans un dashboard (via Python/Streamlit). | Le dashboard doit montrer les indicateurs principaux. | 8 |
| **US5** | Supervision du pipeline | En tant que DevOps Engineer, je veux mettre en place des logs et une supervision des erreurs. | Le système doit notifier en cas d’échec. | 5 |

---

## 🧩 Détail des tâches techniques (Sprint Backlog)

| User Story | Tâche | Responsable | Estimation (SP) | Livrable attendu |
|-------------|-------|--------------|------------------|------------------|
| US1 | Créer le script d’ingestion (Python) | Axel | 3 | Script d’import automatique |
| US1 | Automatiser via un cron job ou scheduler | Kevin | 2 | Script exécuté toutes les heures |
| US2 | Créer le script de nettoyage (Pandas) | Sarah | 3 | Données nettoyées |
| US3 | Concevoir le schéma PostgreSQL | Axel | 3 | Table structurée |
| US3 | Connecter Python à PostgreSQL | Kevin | 2 | Connexion validée |
| US4 | Créer un dashboard Streamlit | Sarah | 5 | Tableau de bord visuel |
| US5 | Ajouter des logs (logging Python) | Kevin | 3 | Fichier de logs |
| US5 | Mettre en place un rapport d’erreurs (email/console) | Ann-Jireh | 2 | Notification d’alerte |

---

## 🕐 Estimation des Story Points (suite de Fibonacci)

| Complexité | Valeur | Description |
|-------------|--------|-------------|
| Très simple | 1 | Configuration rapide ou correction mineure |
| Simple | 2 | Petite fonctionnalité (script, test, doc) |
| Moyenne | 3 | Script avec dépendances ou API |
| Complexe | 5 | Pipeline complet ou dashboard |
| Très complexe | 8 | Intégration multiple ou automatisation avancée |

---

## 🗓️ Planification du Sprint 1

| Sprint | Durée | Objectifs principaux |
|--------|--------|----------------------|
| Sprint 1 | 1 semaine | Mettre en place l’ingestion, le nettoyage et le stockage initial des données. |

**Livrables attendus :**
- Scripts fonctionnels (Python)
- Base PostgreSQL connectée
- Dashboard Streamlit minimal
- Documentation du sprint

---

## 🌀 Événements Scrum simulés

| Événement | Objectif | Durée indicative |
|------------|-----------|------------------|
| **Sprint Planning** | Choisir les US réalisables en 1 semaine | 1h |
| **Daily Scrum** | Suivi quotidien des avancées | 15 min |
| **Sprint Review** | Présenter les livrables | 30 min |
| **Sprint Retrospective** | Identifier les améliorations | 30 min |

---

## 📈 Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
| ✅ Ce qui a bien fonctionné | Bonne communication et répartition des rôles clairs. |
| ⚠️ À améliorer | Estimations parfois sous-évaluées. |
| 🚀 Pour le prochain sprint | Ajouter des tests unitaires et un monitoring plus détaillé. |

---

## 📚 Documentation complémentaire

- Dossier `/docs` : guide d’installation, architecture technique, scripts Python.
- Fichier `/scripts` : contient les scripts d’ingestion et transformation.
- Fichier `/dashboard` : dashboard Streamlit ou Jupyter Notebook.

---

## 🏁 Conclusion

Le sprint 1 permet de poser les bases d’un processus **DataOps automatisé**, garantissant la qualité, la fiabilité et la traçabilité des données à chaque étape du pipeline.
