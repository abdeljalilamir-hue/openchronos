# Protocole de test & validation

## Objectifs

Montrer que le système permet d'**identifier** un véhicule au franchissement d'une ligne,
d'**horodater** son passage avec la précision visée, et de **ne pas produire** de faux
positifs dans un scénario réaliste.

## Références

- Objectifs : `docs/requirements/REQUIREMENTS.md`
- Architecture : `docs/architecture/`
- Protocole radio : `docs/protocol/`

## Matériel nécessaire (si test réel)

- [ ] 2 transpondeurs (minimum)
- [ ] 1 récepteur + dispositif de détection
- [ ] PC / plateforme logicielle
- [ ] Référence chronométrique (ou trigger externe)

## Scénarios de test

### T1. Détection basique
Déplacer un véhicule à vitesse connue → franchissement ligne → horodatage enregistré.

### T2. Multi-transpondeurs
2+ véhicules passent successivement → tous identifiés, ordre préservé.

### T3. Précision temporelle
Comparer horodatage système vs référence. Évaluer écart (moyenne/max).

### T4. Résilience
Passages rapides, proximité, orientation antenne...

## Critères d'acceptation

| Test | Critère | Accepté ? |
|---|---|---|
| T1 | Détection > X % | oui/non |
| T2 | Pas de confusion d'ID | oui/non |
| T3 | Écart < 1 ms (cible à confirmer) | oui/non |
| T4 | Faux positif < 1 % | oui/non |

## Feuille de route

1. **Simulation** (`simulation/`) — valider algorithme / budget de liaison.
2. **Banc de test** (laboratoire) — sans véhicule si possible.
3. **Test terrain** (Motoball Neuvillois) — validation concrète.

## Fichier de compte-rendus

Créer `CR-test-YYYY-MM-DD.md` dans ce dossier à chaque campagne.
