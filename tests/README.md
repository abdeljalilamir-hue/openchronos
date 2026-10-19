# tests/

Tests automatisés (hors protocole de test terrain).

## Distinction
- `docs/validation/TEST-PROTOCOL.md` → **protocole** (scénarios, critères d'acceptation)
- `tests/` → **scripts/tests exécutables** (pytest, unity, etc.)

## Suggestions
- `tests/software/` — tests backend/frontend
- `tests/firmware/` — tests unitaires décodeur/trame
- `tests/integration/` — bout-en-bout (simulé)

> Note : certains modules peuvent aussi avoir leurs propres `tests/`.
