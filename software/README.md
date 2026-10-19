# software/

Plateforme logicielle (hors embarqué).

## Organisation

- `backend/` — API, stockage des temps, traitement, export
- `frontend/` — interface pour visualiser les passages (temps, classement)

## Choix technologiques (à justifier)

Ex. backend : FastAPI (Python) — simple pour traitement/visualisation.
Frontend : Vue/React/Svelte. BDD : SQLite (local) pour prototype, extensible à Postgres.

## API

À documenter via **OpenAPI** (`software/openapi.yaml`) dès qu'une première route existe.
