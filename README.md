# Projet DataTrack – Sprint 1 (DataOps)

## 1. Contexte du projet

Le projet **DataTrack** a pour objectif d’analyser les **performances scolaires des étudiants** à partir du dataset *Students Performance* disponible sur **Kaggle**.  
L’entreprise souhaite mettre en place un pipeline DataOps complet pour automatiser l’analyse et produire des insights clairs sur la réussite scolaire.

### Objectif principal :
Mettre en place un **pipeline automatisé** permettant :
- L’extraction du dataset depuis Kaggle  
- Le nettoyage et la transformation des données  
- Le stockage dans une base de données PostgreSQL  
- La visualisation des résultats dans un **tableau de bord Streamlit**

**But analytique :** Identifier les facteurs qui influencent les scores des étudiants (genre, origine, niveau parental, etc.).

---

## 2. Organisation de l’équipe Scrum

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| Product Owner (PO) | Arcy | Définit les priorités, rédige les User Stories, valide les livrables et gère la documentation. |
| Scrum Master (SM) | Ann-Jireh | Supervise le déroulement du sprint, anime les cérémonies Scrum, s’assure du respect de la méthode (charge légère). |
| DataOps Engineer / Développeur principal | Gloire | Implémente le pipeline complet : extraction, transformation, stockage et visualisation. |

L’équipe fonctionne sur un **sprint d’une semaine**, organisé et suivi via **GitHub Projects (Kanban)**.

---

## 3. Objectifs du Sprint 1

- Identifier les User Stories principales du projet.  
- Détailler les tâches techniques et leur complexité.  
- Planifier les livrables du sprint.  
- Documenter les processus Scrum.  
- Présenter le bilan du sprint (Review + Retrospective).

---

## 4. Organisation GitHub Project

**Nom du projet :** Sprint 1 - DataOps  
**Type :** Tableau Kanban  

**Colonnes :**  
- To do  
- In progress  
- In review  
- Done  

Chaque **issue** correspond à une **User Story (US)** et contient :
- Une description fonctionnelle  
- Les critères d’acceptation  
- Les tâches techniques  
- L’estimation en Story Points  

---

## 5. Product Backlog – User Stories (US)

| ID | User Story | Description | Responsable | Estimation (SP) |
|----|-------------|--------------|--------------|-----------------|
| US1 | Extraction des données depuis Kaggle | Automatiser le téléchargement du dataset *Students Performance*. | Gloire | 5 |
| US2 | Nettoyage et préparation du dataset | Nettoyer et transformer les données brutes pour l’analyse. | Gloire | 3 |
| US3 | Stockage structuré des données | Charger les données nettoyées dans PostgreSQL. | Gloire | 3 |
| US4 | Tableau de bord analytique | Créer un dashboard Streamlit pour visualiser les scores selon différents critères. | Gloire | 8 |
| US5 | Supervision du pipeline | Mettre en place un système de logs pour suivre les exécutions et erreurs. | Ann-Jireh | 2 |
| US6 | Documentation et suivi du sprint | Rédiger la documentation complète du projet et du backlog. | Arcy | 3 |

---

## 6. Détail des tâches techniques (Sprint Backlog)

| User Story | Tâches principales | Responsable | Estimation (SP) | Livrable attendu |
|-------------|-------------------|--------------|------------------|------------------|
| US1 | Télécharger le dataset Kaggle et sauvegarder localement. | Gloire | 5 | Script `extract_kaggle.py` |
| US2 | Nettoyer les colonnes et supprimer les doublons. | Gloire | 3 | Script `clean_data.py` |
| US3 | Créer la base PostgreSQL et charger les données nettoyées. | Gloire | 3 | Script `load_postgres.py` |
| US4 | Concevoir le tableau de bord Streamlit. | Gloire | 8 | Fichier `dashboard.py` |
| US5 | Ajouter un système de logs pour suivre le pipeline. | Ann-Jireh | 2 | Script `logging_system.py` |
| US6 | Rédiger le README.md et la documentation Scrum. | Arcy | 3 | Fichier `docs/Documentation_Scrum.md` |

---

## 7. Estimation des Story Points (Fibonacci)

| Complexité | Valeur | Exemple |
|-------------|--------|----------|
| Très simple | 1 | Ajustement mineur |
| Simple | 2 | Script court ou tâche de configuration |
| Moyenne | 3 | Script d’analyse ou transformation standard |
| Complexe | 5 | Pipeline automatisé |
| Très complexe | 8 | Tableau de bord complet avec intégration |

---

## 8. Planification du Sprint 1

| Sprint | Durée | Objectif principal |
|--------|--------|--------------------|
| Sprint 1 | 1 semaine | Concevoir un pipeline DataOps complet à partir du dataset Kaggle et livrer un tableau de bord fonctionnel. |

**Livrables attendus :**
- Dataset Kaggle téléchargé et nettoyé  
- Base PostgreSQL configurée  
- Tableau de bord Streamlit interactif  
- Documentation Scrum complète  

---

## 9. Événements Scrum simulés

| Événement | Objectif | Durée indicative |
|------------|-----------|------------------|
| Sprint Planning | Identifier les User Stories à réaliser pendant le sprint. | 1h |
| Daily Scrum | Faire le point sur les avancements (via GitHub). | 15 min |
| Sprint Review | Présenter les livrables terminés au Product Owner. | 30 min |
| Sprint Retrospective | Identifier les améliorations pour le prochain sprint. | 30 min |

---

## 10. Bilan du Sprint 1

| Question | Réponse |
|-----------|----------|
| Ce qui a bien fonctionné | Bonne communication et répartition des tâches adaptée à chaque rôle. |
| Ce qui aurait pu mieux se passer | L’extraction depuis Kaggle aurait pu être mieux automatisée. |
| Améliorations à prévoir | Automatiser le téléchargement Kaggle et enrichir le dashboard avec plus d’indicateurs. |

---

## 11. Tableau Sprint Backlog – Synthèse

| User Story | Responsable | Estimation (SP) | Livrable attendu | Statut |
|-------------|--------------|------------------|------------------|--------|
| US1 – Extraction Kaggle | Gloire | 5 | Script `extract_kaggle.py` | In progress |
| US2 – Nettoyage des données | Gloire | 3 | Script `clean_data.py` | To do |
| US3 – Chargement PostgreSQL | Gloire | 3 | Script `load_postgres.py` | To do |
| US4 – Dashboard Streamlit | Gloire | 8 | `dashboard.py` | To do |
| US5 – Supervision / Logs | Ann-Jireh | 2 | `logging_system.py` | Done |
| US6 – Documentation / Backlog | Arcy | 3 | `README.md`, `Documentation_Scrum.md` | Done |

---

## 12. Outils utilisés

| Type | Outil | Rôle |
|------|--------|------|
| Gestion de projet | GitHub Projects | Kanban et backlog |
| Langage | Python | Scripts DataOps |
| Base de données | PostgreSQL | Stockage structuré |
| Visualisation | Streamlit | Tableau de bord analytique |
| Suivi / Logs | Logging Python | Supervision du pipeline |
| Documentation | Markdown | README et doc Scrum |

---

## 13. Répartition de la charge de travail

| Membre | Rôle | Tâches principales | Charge |
|---------|------|-------------------|--------|
| Arcy | Product Owner | Documentation, backlog, validation | Moyenne |
| Ann-Jireh | Scrum Master | Supervision, logs, cérémonies Scrum | Faible |
| Gloire | Développeur DataOps | Extraction, nettoyage, stockage, dashboard | Forte |

---

## 14. Objectif final du Sprint

À la fin du Sprint 1, l’équipe doit avoir :
- Simulé un pipeline DataOps complet et fonctionnel,  
- Livré un tableau de bord analytique clair,  
- Rédigé une documentation Scrum complète,  
- Et démontré la collaboration efficace au sein de l’équipe.

---

## 15. Conclusion

Le projet **DataTrack** illustre la mise en œuvre d’un projet DataOps sous la méthode **Scrum**.  
Grâce à une répartition claire des rôles et un suivi rigoureux, l’équipe a pu planifier, documenter et livrer efficacement un pipeline analytique simulé.

**Équipe 2 – DataTrack**  
Arcy (PO) • Ann-Jireh (SM) • Gloire (Dev DataOps)

*"Inspecter, adapter et livrer de la valeur — même dans la donnée."*
