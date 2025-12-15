# Credit & Climate Risk Lab  
**End-to-end Credit Risk Modeling with Climate Integration**

## 🎯 Objectif du projet
Ce projet démontre une **démarche complète et défendable** de pilotage du risque de crédit, enrichie par l’intégration du **risque climatique (physique et transition)**.

Il couvre l’ensemble de la chaîne :
- estimation du **risque de défaut (PD)**,
- traduction en **impact financier (ECL)**,
- intégration du **climat**,
- **stress tests climatiques**,
- restitution décisionnelle via **Tableau Public**.

Le projet est conçu comme un **cas réel banque / assurance**, orienté **data, risk et décision**.

---

## 🏦 Contexte métier
Le projet se place dans le contexte d’un établissement financier disposant d’un **portefeuille de crédits**.

**Question centrale :**  
> Comment mesurer le risque de crédit, estimer les pertes attendues, et analyser l’impact potentiel du changement climatique sur ce risque afin d’aider au pilotage (Risques / Finance / RSE) ?

Les données utilisées sont **publiques** et servent de **proxies** d’un portefeuille réel.  
L’objectif n’est pas de reproduire un modèle réglementaire interne, mais de démontrer une **méthodologie structurée, explicable et cohérente**.

---

## 📦 Livrables clés

### 🔹 Livrables analytiques
- Probabilité de défaut (**PD**) par prêt
- Perte attendue (**ECL**) par prêt et au niveau portefeuille
- Index d’exposition au **risque climatique physique**
- Résultats de **stress tests climatiques**
- Rapport de **qualité des données**

### 🔹 Livrables décisionnels
Dashboards **Tableau Public** :
1. **Portfolio Overview** (KPI, segmentation du risque)
2. **Climate Physical Exposure** (exposition géographique)
3. **Climate Stress Tests** (baseline vs scénarios)

---

## 🧠 Méthodologie

### 1️⃣ Données & qualité
- Analyse des sources crédit et climat
- Profiling des données
- Gestion des manquants, incohérences et outliers
- Rapport qualité documenté

### 2️⃣ Modélisation du risque de crédit
- Définition explicite du défaut (`default_flag`)
- Sélection des variables explicatives
- Modèle **régression logistique** (standard bancaire)
- Évaluation (AUC, Brier Score)
- **Calibration des probabilités**

### 3️⃣ Traduction financière
- Paramètres EAD / LGD (proxies)
- Calcul de la **Expected Credit Loss (ECL)**
- Agrégation portefeuille

### 4️⃣ Intégration du risque climatique
- Construction d’un **index de risque physique**
- Jointure géographique climat × portefeuille
- Analyse de l’impact climat sur le risque de défaut

### 5️⃣ Stress tests climatiques
- Scénarios :
  - Baseline
  - Transition ordonnée
  - Transition désordonnée
  - Monde chaud
- Ajustement des PD
- Recalcul des ECL
- Analyse des deltas vs baseline

---

## 🧰 Stack technique
- **Python**
- **Jupyter Notebooks** (Notebook-first, pédagogique)
- **Docker** (reproductibilité)
- **scikit-learn**
- **pandas / numpy**
- **Tableau Public** (restitution décisionnelle)
- **Git / GitHub**


## ⚠️ Hypothèses & limites
- Données publiques utilisées comme **proxies**
- LGD et scénarios définis de manière transparente
- Le projet ne remplace pas un modèle réglementaire interne
- Valeur principale : **démarche, cohérence, explicabilité**

---


Ce projet est conçu pour :
- démontrer une **maîtrise du risque de crédit**
- montrer l’intégration concrète du **risque climatique**
- illustrer une capacité à **relier data → modèle → impact financier → décision**

<img width="481" height="512" alt="Screenshot 2025-12-15 at 01 25 28" src="https://github.com/user-attachments/assets/0b85c972-d418-4cb8-a5ea-4391236bd6a2" />

---

## 🚀 Next steps possibles
- Segmentation sectorielle
- Stress tests multi-facteurs
- Intégration transition risk par secteur
- Modèles non-linéaires (benchmark)
- Industrialisation avancée

---

**Auteur** : *Pape Mbacke Thioune*  
**Domaine** : Credit Risk · Climate Risk · Data Science
