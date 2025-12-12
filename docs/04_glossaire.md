# Glossaire (termes métier & data)

## Portefeuille
Ensemble des prêts/clients suivis (la “population” étudiée).

## Défaut
Situation où l’emprunteur ne respecte plus le remboursement. Dans un dataset public, on utilise souvent un statut comme proxy.

## PD (Probability of Default)
Probabilité qu’un prêt tombe en défaut sur un horizon donné.

## EAD (Exposure at Default)
Montant exposé au moment du défaut. Proxy fréquent : montant du prêt restant dû (ou loan_amnt dans un dataset public).

## LGD (Loss Given Default)
Pourcentage perdu si défaut. Exemple : LGD=60% signifie qu’on récupère 40% et qu’on perd 60%.

## ECL (Expected Credit Loss)
Perte attendue : ECL = PD × LGD × EAD (simplifié). Sert à exprimer le risque en euros.

## Calibration
Technique pour rendre les probabilités fiables (si le modèle dit 20%, on veut que ~20% défaut réellement).

## Risque climatique physique
Risque lié aux événements climatiques (inondations, incendies, tempêtes…). Souvent dépendant de la localisation.

## Risque de transition
Risque lié à la transition bas-carbone (réglementation, prix énergie, taxe carbone, chocs sectoriels).

## Stress test
Simulation d’un futur défavorable (scénario) pour mesurer l’impact sur le risque et les pertes.

## Proxy
Approximation mesurable utilisée lorsque la vraie variable métier n’est pas disponible (courant sur données publiques).

