# Documentation Scrum – Projet DataOps : Analyse des performances scolaires des étudiants

---

## 1. Contexte du projet

L’entreprise souhaite suivre les performances scolaires des étudiants à l’aide d’un tableau de bord analytique.  
Pour cela, l’équipe Data doit concevoir un pipeline DataOps automatisé permettant de télécharger, transformer et analyser les données issues du dataset Kaggle :  
**Students Performance Dataset**

Ce dataset contient des informations sur :
- les scores des étudiants,
- leur genre,
- leur origine ethnique,
- le niveau d’éducation des parents,
- le type de repas pris avant les tests, etc.

Objectif analytique : Identifier les patterns et les facteurs influençant la réussite scolaire des élèves.

---

## 2. Organisation Scrum

| Rôle | Membre | Responsabilités principales |
|------|---------|-----------------------------|
| Product Owner | Gloire | Définit la vision produit, gère le backlog et les priorités |
| Scrum Master | Arcy | Facilite les rituels Scrum, supervise le bon déroulement du sprint |
| Data Engineer (support) | Ann-Jireh | Contribue à la documentation et à la vérification du tableau de bord (charge réduite) |

---

## 3. Product Backlog – User Stories

### US1 – Extraction des données depuis Kaggle
**En tant que** Data Engineer,  
**je veux** télécharger automatiquement le dataset *Students Performance* depuis Kaggle,  
**afin de** disposer des données sources pour le pipeline.

**Critères d’acceptation :**
- Le dataset est bien téléchargé depuis Kaggle.
- Les fichiers sont stockés dans un dossier `/data/raw`.
- Le fichier CSV est exploitable.

**Estimation :** 3 Story Points  
**Responsable :** Gloire

---

### US2 – Nettoyage et préparation des données
**En tant que** Analyste Data,  
**je veux** nettoyer et structurer les données,  
**afin de** supprimer les valeurs manquantes et garantir la qualité du dataset.

**Critères d’acceptation :**
- Aucune valeur nulle dans les colonnes critiques.
- Données cohérentes et typées correctement.
- Export d’un fichier `cleaned_data.csv`.

**Estimation :** 5 Story Points  
**Responsable :** Gloire

---

### US3 – Chargement des données dans l’environnement analytique
**En tant que** Data Engineer,  
**je veux** simuler le chargement des données dans une base de données,  
**afin de** permettre l’alimentation du futur tableau de bord.

**Critères d’acceptation :**
- Schéma ETL décrit et validé.
- Étape de chargement documentée dans le pipeline.

**Estimation :** 3 Story Points  
**Responsable :** Arcy

---

### US4 – Création du tableau de bord analytique
**En tant que** Analyste,  
**je veux** concevoir un tableau de bord avec des visualisations claires,  
**afin de** mettre en évidence les corrélations entre les notes, le genre, et le niveau d’éducation parental.

**Critères d’acceptation :**
- Le dashboard comporte au moins trois graphiques pertinents (ex : histogramme, corrélation, heatmap).
- L’interprétation des résultats est rédigée.
- Le rendu final est compréhensible sans code.

**Estimation :** 5 Story Points  
**Responsable :** Arcy

---

### US5 – Documentation et bilan du sprint
**En tant que** membre de l’équipe,  
**je veux** rédiger la documentation du projet et le bilan du sprint,  
**afin de** assurer la traçabilité du travail et la transparence de l’équipe Scrum.

**Critères d’acceptation :**
- README.md et documentation_scrum.md complets.
- Rétrospective du sprint incluse.
- Livrables finalisés et déposés sur GitHub.

**Estimation :** 2 Story Points  
**Responsable :** Ann-Jireh

---

## 4. Estimation et priorisation (Backlog priorisé)

| ID | User Story | Priorité | Story Points | Responsable |
|----|-------------|-----------|---------------|--------------|
| US1 | Extraction du dataset Kaggle | Haute | 3 | Gloire |
| US2 | Nettoyage et transformation | Très haute | 5 | Gloire |
| US3 | Chargement simulé | Moyenne | 3 | Arcy |
| US4 | Dashboard analytique | Très haute | 5 | Arcy |
| US5 | Documentation finale | Basse | 2 | Ann-Jireh |

---

## 5. Sprint Planning (Semaine 1)

**Durée du sprint :** 1 semaine  
**Objectif du Sprint :** Disposer d’un pipeline complet documenté et d’un dashboard analytique opérationnel.

| Tâche | Description | Responsable | Story Points | Livrable attendu |
|-------|--------------|--------------|---------------|------------------|
| T1 | Télécharger le dataset depuis Kaggle | Gloire | 3 | students_performance.csv |
| T2 | Nettoyer et structurer les données | Gloire | 5 | cleaned_data.csv |
| T3 | Documenter le pipeline ETL | Arcy | 3 | Schéma ETL |
| T4 | Créer le tableau de bord (maquette) | Arcy | 5 | Dashboard PDF ou capture |
| T5 | Rédiger la documentation finale | Ann-Jireh | 2 | documentation_scrum.md complet |

---

## 6. Sprint Backlog – Vue synthétique

| Tâche | Statut | Responsable | Points | État |
|-------|---------|--------------|---------|-------|
| T1 – Extraction Kaggle | Terminé | Gloire | 3 | Done |
| T2 – Nettoyage | En cours | Gloire | 5 | In progress |
| T3 – Chargement simulé | Terminé | Arcy | 3 | Done |
| T4 – Dashboard | En revue | Arcy | 5 | In review |
| T5 – Documentation | À faire | Ann-Jireh | 2 | To do |

---

## 7. Événements Scrum simulés

| Événement | Objectif | Durée | Responsable |
|------------|-----------|--------|--------------|
| Sprint Planning | Planifier les tâches et définir le Sprint Goal | 30 min | Arcy |
| Daily Scrum | Suivi rapide de l’avancement | 10 min/jour | Gloire |
| Sprint Review | Présenter les résultats du pipeline et du dashboard | 20 min | Arcy |
| Sprint Retrospective | Identifier les points à améliorer | 15 min | Ann-Jireh |

---

## 8. Bilan du Sprint

| Question | Réponse |
|-----------|----------|
| Ce qui a bien fonctionné | Répartition claire des rôles, bonne communication, respect des délais |
| Ce qui aurait pu mieux se passer | Estimation initiale des tâches légèrement sous-évaluée |
| Ce qu’on va améliorer | Documenter les étapes plus tôt et inclure des exemples visuels dans le README |

---

## 9. Conclusion

Ce premier sprint a permis de :
- Simuler un pipeline DataOps complet (Extraction → Nettoyage → Chargement → Analyse).
- Produire un tableau de bord analytique lisible et argumenté.
- Structurer la documentation Scrum de manière claire et collaborative.

La prochaine itération visera à approfondir les analyses et à automatiser davantage le processus.

---

### Fichiers livrables finaux :
- README.md → Présentation du projet et de l’équipe  
- documentation_scrum.md → Organisation Scrum complète  
- dashboard.png ou dashboard.pdf → Résultat visuel final  
- cleaned_data.csv → Dataset nettoyé (simulation)

---

Équipe DataPulse :
- Gloire — Product Owner  
- Arcy — Scrum Master  
- Ann-Jireh — Data Engineer (documentation)
