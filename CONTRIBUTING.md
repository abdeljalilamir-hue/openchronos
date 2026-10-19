# Contribuer à OpenChronos

Merci de votre intérêt pour le projet ! Ce document décrit comment nous organisons le travail.

## 🌿 Branches

- `main` — toujours stable, contient le dernier état validé.
- `docs/<sujet>` — rédaction / documentation (ex. `docs/requirements`).
- `feat/<sujet>` — fonctionnalité matérielle, firmware ou logicielle.
- `fix/<sujet>` — correction.

Convention de nom de branche : `type/kebab-case-court` (ex. `docs/adr-001-rf-433`, `feat/rx-decoder`).

## 📝 Commits

Format [Conventional Commits](https://www.conventionalcommits.org/) :

```
<type>(<portée>) : <description courte>

type ∈ feat | fix | docs | refactor | test | chore | hardware | firmware
```

Exemples :
- `docs(requirements) : chiffrer la précision visée à 1 ms`
- `feat(receiver) : ajouter le décodage CRC32`

## 🔄 Pull Requests

1. Ouvrir une branche à partir de `main`.
2. Une PR = **un livrable ou une décision** documentée.
3. Décrire le **pourquoi** dans la PR (pas seulement le quoi).
4. Si la PR change une décision technique → mettre à jour ou créer un **ADR** (voir `docs/architecture/adr/`).
5. Revue par au moins un autre membre avant merge.

## 🧪 Tests

- Les tests automatisés vivent dans `tests/` et dans chaque module (`firmware/*/tests`, `software/*/tests`).
- Le **protocole de test** (document) vit dans `docs/validation/`.
- `simulation/` permet de valider le traitement du signal **avant** tout matériel.

## 📚 Documentation

- Toute décision technique majeure → **ADR** dans `docs/architecture/adr/`.
- Tout besoin chiffré → `docs/requirements/`.
- Le projet vise des livrables notés : **traçabilité > quantité de code**.

## ✅ Checklist avant PR

- [ ] Le code se construit / s'exécute.
- [ ] Les tests pertinents passent.
- [ ] La doc est à jour (README, ADR si décision).
- [ ] Pas de fichier sensible (mot de passe, token) versionné.
