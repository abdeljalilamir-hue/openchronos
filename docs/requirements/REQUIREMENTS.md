# Besoins chiffrés

Objectif : traduire le besoin fonctionnel en **ordres de grandeur quantifiés** pour orienter
le choix technologique et rendre le protocole de test objectif.

## Hypothèses terrain (Motoball Neuvillois)

À remplir au fil du projet (recueil terrain / cadrage).

## 1) État de l'art / contraintes
- Vitesse max visée : **? km/h** (→ m/s)
- Nombre de véhicules simultanés : **?**
- Portée nécessaire (ligne → véhicule) : **? m**
- Franchissement ligne = instant à détecter : **précision souhaitée ? ms**

## 2) Ordres de grandeur à estimer

| Besoin | Valeur visée | Justification |
|---|---|---|
| Précision temporelle | — | impact sur classement (1 ms suffit-il ?) |
| Temps de passage ligne | — | delta t mini entre 2 véhicules |
| Portée radio | — | voir lignes, obstacles |
| Latence détection → horodatage | — | doit être négligeable vs précision |
| Autonomie transpondeur | — | course / séance |
| Immunité aux interférences | — | plusieurs transpondeurs / autres émetteurs |

## 3) Indicateurs de réussite (KPI)

| KPI | Cible | Test à mettre en œuvre |
|---|---|---|
| Précision horodatage | < 1 ms (à discuter) | Comparaison avec référence (trigger, chronomètre) |
| Taux de détection correcte | > 99 % | Essais sur N passages |
| Taux de faux positifs | < 1 % | Essais hors-ligne + multi-véhicules |
| Nombre simultané supporté | >= N | Scénario congestion |

## 4) Premiers calculs (à compléter)

### Budget de liaison (à compléter dans `simulation/`)
- Puissance TX, gain antennes, pertes, sensibilité RX → marge.
- Voir `simulation/budget_liaison.ipynb` (à créer).

### Temps de détection
- Vitesse V (m/s), longueur zone de détection (m) → temps en zone.

## Références
- OpenSTINT : https://openstint.org/
- Cadrage avec Motoball Neuvillois
