# Documentation Scrum — Projet DataTrack (Sprint 1 - DataOps)

---

## 1. Contexte du projet

Le projet **DataTrack** s’inscrit dans une démarche **DataOps** visant à automatiser le suivi et l’analyse des performances scolaires des étudiants à partir du dataset **Students Performance (Kaggle)**.  
Ce dataset contient des informations telles que les **scores**, le **genre**, l’**origine ethnique**, le **niveau d’éducation des parents**, et d’autres facteurs.

### Objectif principal :
Mettre en place une organisation Scrum simulée autour d’un **pipeline DataOps complet** permettant :
- L’extraction des données depuis Kaggle,
- Le nettoyage et la transformation du dataset,
- Le stockage structuré dans une base PostgreSQL,
- La visualisation des résultats dans un tableau de bord Streamlit.

Ce sprint permet de démontrer la mise en œuvre concrète de la **méthodologie Agile Scrum** appliquée à un projet Data.

---

## 2. Équipe et rôles Scrum

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| **Product Owner (PO)** | **Arcy** | Définit les priorités du backlog, valide les livrables, rédige la documentation et gère la vision produit. |
| **Scrum Master (SM)** | **Ann-Jireh** | Facilite la méthode Scrum, veille à la communication et anime les réunions (faible charge de travail technique). |
| **DataOps Engineer / Développeur principal** | **Gloire** | Conçoit et implémente le pipeline complet : extraction, nettoyage, stockage et visualisation. |

**Organisation :**
- L’équipe travaille en sprint d’une semaine.  
- Les réunions Scrum sont simulées via des mises à jour sur GitHub (issues, Kanban et backlog).  
- Le suivi des tâches est effectué à l’aide du **Project Board GitHub**.

---

## 3. Les artefacts Scrum

### 3.1 Product Backlog
Le **Product Backlog** regroupe l’ensemble des besoins du projet sous forme de **User Stories (US)**.

| ID | User Story | Description | Responsable | Estimation (SP) |
|----|-------------|--------------|--------------|-----------------|
| US1 | Extraction des données depuis Kaggle | Télécharger et sauvegarder le dataset Kaggle pour alimenter le pipeline. | Gloire | 5 |
| US2 | Nettoyage et préparation du dataset | Nettoyer et transformer les données pour les rendre exploitables. | Gloire | 3 |
| US3 | Stockage structuré des données | Charger les données nettoyées dans une base PostgreSQL. | Gloire | 3 |
| US4 | Tableau de bord analytique | Visualiser les données avec Streamlit. | Gloire | 8 |
| US5 | Supervision du pipeline | Créer un système de logs et suivi des erreurs. | Ann-Jireh | 2 |
| US6 | Documentation et suivi du sprint | Rédiger la documentation et maintenir le backlog. | Arcy | 3 |

---

### 3.2 Sprint Backlog

| User Story | Tâches principales | Responsable | Estimation (SP) | Livrable attendu |
|-------------|-------------------|--------------|------------------|------------------|
| US1 | Télécharger le dataset Kaggle et sauvegarder localement. | Gloire | 5 | Script `extract_kaggle.py` |
| US2 | Nettoyer les données et supprimer les doublons. | Gloire | 3 | Script `clean_data.py` |
| US3 | Créer la base PostgreSQL et insérer les données. | Gloire | 3 | Script `load_postgres.py` |
| US4 | Concevoir le dashboard Streamlit. | Gloire | 8 | Fichier `dashboard.py` |
| US5 | Mettre en place le système de logs. | Ann-Jireh | 2 | `logging_system.py` |
| US6 | Rédiger la documentation et le bilan du sprint. | Arcy | 3 | `README.md`, `Documentation_Scrum.md` |

---

### 3.3 L’incrément
L’**incrément** représente le résultat du sprint, c’est-à-dire :
- Un pipeline DataOps complet simulé,  
- Une documentation claire et fonctionnelle,  
- Des User Stories validées par le Product Owner,  
- Un tableau de bord de suivi de l’équipe sur GitHub (Kanban).  

---

## 4. Les événements Scrum simulés

| Événement | Objectif | Durée | Responsable |
|------------|-----------|--------|--------------|
| **Sprint Planning** | Identifier les User Stories du sprint et définir les objectifs. | 1 heure | Arcy |
| **Daily Scrum** | Suivre les avancements (simulé via mise à jour des issues). | 15 minutes | Ann-Jireh |
| **Sprint Review** | Présenter les livrables à la fin du sprint (scripts, docs, dashboard). | 30 minutes | Arcy |
| **Sprint Retrospective** | Identifier ce qui a bien fonctionné et ce qui doit être amélioré. | 30 minutes | Ann-Jireh |

---

## 5. Estimation en Story Points (Suite de Fibonacci)

| Niveau de complexité | Valeur | Description |
|-----------------------|--------|--------------|
| Très simple | 1 | Tâche mineure ou ajustement de code |
| Simple | 2 | Petite fonctionnalité (ex : script court, logs) |
| Moyenne | 3 | Script standard ou transformation simple |
| Complexe | 5 | Automatisation de pipeline ou script API |
| Très complexe | 8 | Intégration complète (dashboard, visualisation) |

---

## 6. Cycle du Sprint

1. **Sprint Planning** → définition des User Stories à réaliser.  
2. **Daily Scrum** → suivi régulier de l’avancement (via Kanban GitHub).  
3. **Développement** → réalisation des tâches techniques.  
4. **Sprint Review** → présentation des livrables et validation.  
5. **Sprint Retrospective** → bilan du sprint et axes d’amélioration.

### Représentation schématique :

---

## 7. Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
| Ce qui a bien fonctionné | Répartition claire des rôles, bon suivi via GitHub Projects. |
| Ce qui aurait pu mieux se passer | L’extraction Kaggle aurait pu être mieux automatisée. |
| Améliorations envisagées | Ajouter une extraction API Kaggle automatique et plus de visualisations sur le dashboard. |

---

## 8. Outils utilisés

| Type | Outil | Rôle |
|------|--------|------|
| Gestion de projet | GitHub Projects | Kanban et backlog du sprint |
| Documentation | Markdown | README et docs Scrum |
| Environnement | Python | Simulation du pipeline DataOps |
| Base de données | PostgreSQL | Stockage des données nettoyées |
| Visualisation | Streamlit | Tableau de bord analytique |
| Supervision | Logging (Python) | Suivi des erreurs et des étapes |

---

## 9. Objectif final du projet

À la fin du Sprint 1, l’équipe doit être capable de démontrer :
- La simulation complète d’un **pipeline DataOps** (de l’extraction à la visualisation),  
- Une **organisation Scrum claire et documentée**,  
- Un **travail collaboratif efficace** avec répartition équilibrée des tâches.

---

## 10. Conclusion

Le projet **DataTrack** démontre comment les principes Scrum peuvent être appliqués dans un environnement DataOps.  
Grâce à la coordination entre le Product Owner (Arcy), le Scrum Master (Ann-Jireh) et le Développeur principal (Gloire), l’équipe a pu simuler un sprint Agile complet, livrer des artefacts clairs et assurer un suivi transparent du cycle de développement.

---

**Équipe 2 - DataTrack**  
Arcy (PO) – Ann-Jireh (SM) – Gloire (Dev DataOps)

_"Inspecter, adapter et livrer de la valeur — même dans la donnée."_
