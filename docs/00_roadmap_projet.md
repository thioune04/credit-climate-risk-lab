# Roadmap projet — Credit & Climate Risk Lab

## Objectif global
Construire un projet de bout en bout (Notebook-first) qui permet de :
1) mesurer le risque de crédit (PD),
2) traduire en impact financier (ECL),
3) intégrer le risque climatique (physique + transition),
4) produire des stress tests,
5) restituer via Tableau Public.

## Contraintes projet
- Travail principal dans Jupyter Notebooks (pédagogique, présentable).
- Environnement reproductible via Docker.
- Restitution décisionnelle via Tableau Public.
- Aucune donnée brute versionnée sur Git (conformité).

## Phases
### Phase 0 — Cadrage & setup
- Cadrage métier (problème, risques, enjeux)
- Objectifs et livrables attendus
- Choix outils & justification
- Plan d’exécution (notebooks)

### Phase 1 — Données (compréhension)
- Identifier les sources (crédit + climat)
- Charger et profiler les données (shape, colonnes, valeurs)
- Dictionnaire de données (colonnes → sens métier)

### Phase 2 — Qualité data (banque/assurance)
- Manquants, formats, cohérences
- Outliers (valeurs aberrantes)
- Mini rapport qualité + décisions (imputer/supprimer/capper)

### Phase 3 — Target & features (préparation modèle)
- Définir la cible défaut (default_flag)
- Sélection des variables explicatives
- Encodage catégories, imputation, sauvegarde X/y

### Phase 4 — Modèle PD (probabilité de défaut)
- Modèle explicable (logistique)
- Évaluation (AUC, calibration)
- Export métriques + graphiques

### Phase 5 — Traduction financière (ECL simplifiée)
- Définir EAD, LGD (proxies)
- Calcul ECL par prêt et agrégation portefeuille
- Exports décisionnels

### Phase 6 — Risque physique (climat)
- Construire index d’exposition physique (FEMA NRI)
- Relier exposition à la géographie du portefeuille
- Export exposition + visualisations

### Phase 7 — Risque transition (stress tests)
- Définir scénarios (baseline / orderly / disorderly / hot house)
- Ajuster PD, recalculer ECL
- Comparer baseline vs scénarios

### Phase 8 — Tableau Public (restitution)
- Créer exports “Tableau-ready”
- Dashboards : Portfolio / Physical / Stress

### Phase 9 — Storytelling entretien
- Pitch 60s + Q/R
- Limites & next steps

