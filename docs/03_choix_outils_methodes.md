# Choix des outils & méthodes

## 1) Jupyter Notebooks (Notebook-first)
### Définition
Un notebook est un document qui mélange texte + code + résultats.
### Pourquoi
- Pédagogique : on explique chaque étape.
- Traçable : on voit les sorties.
- Présentable : parfait en entretien et en mission.
### Usage
Toutes les transformations et analyses clés sont réalisées dans des notebooks dédiés, avec exports de rendus.

## 2) Docker (reproductibilité)
### Définition
Docker encapsule l’environnement (Python + librairies) dans un conteneur.
### Pourquoi
- Évite les problèmes “ça marche chez moi”.
- Montre une maturité pro (industrialisation légère).
### Usage
On lance Jupyter via Docker et on exécute les notebooks dans un environnement stable.

## 3) Tableau Public (restitution décisionnelle)
### Définition
Outil de visualisation pour construire des dashboards interactifs.
### Pourquoi
- Les décideurs veulent des KPI + cartes + comparatifs.
- Permet de montrer l’impact des scénarios en quelques vues.
### Usage
On exporte des CSV “Tableau-ready” (propres, simples, noms clairs) depuis les notebooks.

## 4) Méthodologie de modélisation (explicable)
### Choix modèle PD
Régression logistique + calibration.
### Pourquoi
- Explicable, standard en risque.
- Défendable (compréhension des drivers).
### Limites assumées
Les paramètres EAD/LGD sont des proxies (données publiques). La valeur est dans la démarche complète et la transparence.

