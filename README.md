# project-datatrack-equipe2  
**TP DataOps — Suivi des performances scolaires des étudiants (Scrum Simulation)**  

---

# Projet DataTrack - Sprint 1 (DataOps)

---

## Contexte du projet

L’entreprise souhaite mieux comprendre les **facteurs influençant la réussite scolaire** des étudiants.  
Pour cela, elle veut mettre en place un **pipeline DataOps automatisé** capable de :

- Extraire le dataset depuis **Kaggle** (*Students Performance Dataset*),  
- Nettoyer et transformer les données (scores, genre, origine ethnique, niveau parental…),  
- Charger ces données dans une base centralisée,  
- Et les visualiser dans un **tableau de bord analytique**.  

 **Objectif final :** identifier des *patterns et insights* liés à la réussite scolaire (par exemple : influence du niveau parental sur les scores).

---

##  Organisation Scrum de l’équipe

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| **Product Owner (PO)** | **Arcy** | Définit les priorités, rédige les User Stories, valide les livrables. |
| **Scrum Master (SM)** | **Ann-Jireh** | Facilite la méthode Scrum, anime les réunions, supervise le sprint (faible charge). |
| **DataOps Engineer / Développeur principal** | **Gloire** | Met en place le pipeline complet : extraction, transformation, chargement, visualisation. |

 *Ann-Jireh* a une mission légère de coordination, sans tâches techniques lourdes.  
La majorité du travail technique est assurée par *Gloire*, sous la supervision d’*Arcy* (PO).

---

##  Objectifs du Sprint 1

- Simuler un sprint Scrum complet (1 semaine).  
- Identifier et décrire les User Stories principales.  
- Détailler les tâches techniques et leur complexité.  
- Planifier le sprint et répartir les responsabilités.  
- Documenter le travail collaboratif (README + Scrum doc).  

---

##  Organisation GitHub Project

**Nom du projet :** `Sprint 1 - DataOps`  
**Type :** Kanban Board  

**Colonnes :**
- To do  
- In progress  
- In review  
- Done  

Chaque **issue** = une **User Story (US)**  
Chaque US contient :  
→ Détail de la fonctionnalité  
→ Critères d’acceptation  
→ Tâches techniques  

---

##  Product Backlog — User Stories (US)

| ID | User Story | Description | Responsable | Estimation (SP) |
|----|-------------|--------------|--------------|-----------------|
| **US1** | Extraction des données depuis Kaggle | En tant que DataOps Engineer, je veux automatiser le téléchargement du dataset depuis Kaggle pour alimenter le pipeline. | **Gloire** | 5 |
| **US2** | Nettoyage et préparation du dataset | En tant que DataOps Engineer, je veux nettoyer et transformer les données pour qu’elles soient prêtes à l’analyse. | **Gloire** | 3 |
| **US3** | Stockage structuré des données | En tant que DataOps Engineer, je veux charger les données nettoyées dans une base PostgreSQL pour les rendre accessibles. | **Gloire** | 3 |
| **US4** | Tableau de bord analytique | En tant qu’analyste, je veux visualiser les scores par genre, origine, et niveau parental dans un dashboard Streamlit. | **Gloire** | 8 |
| **US5** | Supervision du pipeline | En tant que Scrum Master, je veux un système de logs et suivi du pipeline pour détecter les erreurs. | **Ann-Jireh** | 2 |
| **US6** | Documentation et suivi du sprint | En tant que Product Owner, je veux rédiger la documentation du projet et suivre le backlog. | **Arcy** | 3 |

---

##  Détail des tâches techniques (Sprint Backlog)

| User Story | Tâches | Responsable | Estimation (SP) | Livrable attendu |
|-------------|--------|--------------|------------------|------------------|
| **US1** | Télécharger le dataset Kaggle (API ou manuel), sauvegarder localement. | Gloire | 3 | Dataset brut (`/data/raw/students_performance.csv`) |
| **US1** | Définir le dossier de travail et les logs de téléchargement. | Gloire | 2 | Script `extract_kaggle.py` |
| **US2** | Nettoyer les colonnes (valeurs manquantes, doublons). | Gloire | 3 | Script `clean_data.py` |
| **US3** | Créer la base PostgreSQL et les tables `students_raw` / `students_clean`. | Gloire | 3 | Script `load_postgres.py` |
| **US4** | Créer le dashboard Streamlit : histogrammes et moyennes par catégorie. | Gloire | 8 | `dashboard.py` (Streamlit) |
| **US5** | Ajouter un fichier de logs (suivi des étapes et erreurs). | Ann-Jireh | 2 | `logging_system.py` |
| **US6** | Rédiger le `README.md`, la doc Scrum et le backlog du sprint. | Arcy | 3 | `docs/Documentation_Scrum.md` |

---

##  Estimation des Story Points (suite de Fibonacci)

| Complexité | Valeur | Exemple |
|-------------|--------|----------|
| Très simple | 1 | Ajustement ou test mineur |
| Simple | 2 | Script court ou tâche légère |
| Moyenne | 3 | Script standard (nettoyage, chargement) |
| Complexe | 5 | Pipeline complet ou automatisation |
| Très complexe | 8 | Dashboard ou intégration complète |

---

##  Planification du Sprint 1

| Sprint | Durée | Objectif principal |
|--------|--------|--------------------|
| **Sprint 1** | 1 semaine | Concevoir le pipeline complet du dataset Kaggle et livrer un tableau de bord fonctionnel. |

### 🎯 Livrables attendus :
- Dataset téléchargé depuis Kaggle  
- Données nettoyées et stockées dans PostgreSQL  
- Dashboard Streamlit avec indicateurs clés  
- Documentation complète du sprint  

---

##  Événements Scrum simulés

| Événement | Objectif | Durée indicative |
|------------|-----------|------------------|
| **Sprint Planning** | Planifier les US à réaliser dans le sprint | 1h |
| **Daily Scrum** | Faire le point sur les avancements (simulé) | 15 min |
| **Sprint Review** | Présenter les livrables au Product Owner | 30 min |
| **Sprint Retrospective** | Identifier les améliorations possibles | 30 min |

---

##  Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
|  Ce qui a bien fonctionné | Bonne coordination et répartition claire du travail. |
|  Ce qui aurait pu mieux se passer | Le téléchargement du dataset a pris plus de temps que prévu. |
|  Améliorations pour le prochain sprint | Automatiser totalement l’extraction Kaggle via API et ajouter plus de visualisations. |

---

## Tableau Sprint Backlog — Synthèse

| User Story | Responsable | Estimation (SP) | Livrable attendu | Statut |
|-------------|--------------|------------------|------------------|--------|
| **US1 – Extraction Kaggle** | Gloire | 5 | Script `extract_kaggle.py` | 🟡 In progress |
| **US2 – Nettoyage des données** | Gloire | 3 | Script `clean_data.py` | 🔵 To do |
| **US3 – Chargement PostgreSQL** | Gloire | 3 | Script `load_postgres.py` | 🔵 To do |
| **US4 – Dashboard Streamlit** | Gloire | 8 | `dashboard.py` | 🔵 To do |
| **US5 – Supervision / Logs** | Ann-Jireh | 2 | `logging_system.py` | 🟢 Done |
| **US6 – Documentation / Backlog** | Arcy | 3 | `README.md`, `Documentation_Scrum.md` | 🟢 Done |

---

##  Documentation Scrum intégrée

###  Principes clés
Scrum repose sur trois piliers : **transparence**, **inspection**, **adaptation**.  
Chaque sprint vise à produire un livrable fonctionnel, à inspecter le résultat et à s’améliorer.

---

###  Rôles Scrum
- **Product Owner (Arcy)** : fixe les priorités et valide les livrables.  
- **Scrum Master (Ann-Jireh)** : anime les cérémonies et veille à la méthode (faible charge).  
- **Développeur DataOps (Gloire)** : réalise la majorité des tâches techniques.

---

###  Cycle du Sprint
---

###  Objectif final
À la fin du Sprint 1, l’équipe doit :
- Avoir simulé un **pipeline DataOps complet**,  
- Livré une documentation claire et structurée,  
- Et démontré sa capacité à travailler en mode **Scrum**.

---

>  *“Inspecter, adapter et livrer de la valeur — même dans la donnée.”*  
> — Équipe 2 : **Arcy**, **Ann-Jireh**, **Gloire**
