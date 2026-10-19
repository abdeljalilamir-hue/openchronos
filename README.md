# OpenChronos

> **Conception d'une solution open source de chronométrage sportif par transpondeur**

Projet encadré par **Mickaël BARON** — [ISAE-ENSMA](https://www.isae-ensma.fr) / [LIAS](https://www.lias-lab.fr) (EA 6315) — Promotion 2027.

---

## 🎯 Contexte

Le chronométrage sportif pour les sports motorisés (moto, karting, cyclisme…) repose aujourd'hui sur des systèmes **propriétaires coûteux** (transpondeurs + boucles de détection), verrouillant circuits et organisateurs dans des écosystèmes fermés, avec des coûts élevés et une dépendance à des fournisseurs uniques.

Une initiative open source existe ([OpenSTINT](https://openstint.org/)) mais elle est dédiée aux modèles réduits. **Aucune solution ouverte, documentée, réplicable et validée n'existe à ce jour pour des véhicules de taille réelle.**

OpenChronos vise à combler ce vide, en partenariat terrain avec le club **Motoball Neuvillois**.

## 🧭 Question de recherche

*Comment concevoir une solution de chronométrage open source, fiable, accessible et reproductible pour des véhicules de taille réelle, tout en garantissant une identification précise des concurrents et une évolution possible du système ?*

## 🧩 Éléments du système

- **Transpondeurs embarqués** sur les motos / véhicules
- **Dispositif de détection** installé au niveau de la ligne de chronométrage
- **Système de réception / décodage** pour identifier le transpondeur au passage
- **Plateforme logicielle** pour enregistrer, stocker, traiter et visualiser les temps
- **Boîtiers et supports mécaniques** adaptés au circuit ou au terrain

## 📦 Livrables

1. Description du fonctionnement général du système
2. Architecture globale (transpondeurs, détection, logiciel)
3. Étude des technologies + justification des choix
4. Schémas ou maquettes des différents éléments
5. Proposition de fonctionnement de la plateforme logicielle
6. Estimation des performances attendues et des coûts
7. Identification du matériel nécessaire pour une réalisation ultérieure
8. Protocole de test et de validation
9. Documentation permettant de poursuivre le projet

## 📁 Structure du dépôt

```
openchronos/
├── README.md
├── LICENSE                 # Licence MIT (logiciel / firmware)
├── LICENSES/               # Licences dédiées (hardware, documentation)
├── CONTRIBUTING.md
├── CHANGELOG.md
├── docs/
│   ├── subject/            # Le sujet officiel + résumé
│   ├── requirements/       # Besoins chiffrés (vitesse, précision, portée…)
│   ├── architecture/       # Schémas globaux + ADR (décisions)
│   ├── protocol/           # Trame radio, identification, synchronisation
│   ├── technology-study/   # Étude des technologies + justification
│   ├── cost-performance/   # Estimation coûts & performances
│   └── validation/         # Protocole de test
├── hardware/               # Électronique (transpondeur, récepteur, BOM)
├── firmware/               # Code embarqué (transponder, receiver, common)
├── software/               # Plateforme logicielle (backend, frontend)
├── mechanical/             # CAO, boîtiers, supports (impression 3D)
├── simulation/             # Notebooks, budget de liaison, essais signal
├── tests/                  # Tests automatisés
└── assets/                 # Images, logos
```

## 🚀 Pour démarrer

> **Statut** : phase de cadrage. Les dossiers `firmware/`, `software/`, `mechanical/` sont des squelettes à remplir dès qu'un premier résultat y atterrit.

Voir `docs/requirements/` pour les besoins chiffrés et `docs/architecture/adr/` pour l'historique des choix techniques.

## 🤝 Contribuer

Lire [`CONTRIBUTING.md`](CONTRIBUTING.md). En résumé : une branche par sujet, une PR = un livrable ou une décision documentée.

## 📄 Licence

- **Logiciel / firmware** : MIT (voir [`LICENSE`](LICENSE))
- **Hardware** : CERN-OHL-S (voir [`LICENSES/`](LICENSES/))
- **Documentation / mécanique** : CC-BY-SA (voir [`LICENSES/`](LICENSES/))

---

*Ce dépôt documente la conception d'un prototype fonctionnel, documenté et reproductible — pas nécessairement un produit industrialisé.*
