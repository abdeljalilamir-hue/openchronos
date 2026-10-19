# Protocole radio

Ce dossier contient la **spécification technique** du lien radio (cœur du projet).

## À définir (ordre de priorités)

1. **Bande & fréquence** — ISM autorisée en France ? (433 MHz, 868 MHz, 2.4 GHz...)
2. **Modulation** — OOK, FSK, GFSK, LoRa...
3. **Débit (bitrate)** — compromis portée/précision/robustesse
4. **Format trame** — préambule, sync, ID (UID), CRC, éventuel compteur
5. **Identification** — unique par transpondeur, anti-collision ?
6. **Synchronisation / horodatage** — quand horodater ? (réception RX) + jitter
7. **Gestion multi-transpondeurs** — TDMA ? CSMA ? simple broadcast + déduplication ?

## Fichiers à créer

- `frequency.md` — choix fréquence + justification
- `frame-format.md` — schéma bit à bit
- `collision-handling.md` — stratégie multi-transpondeurs
- `timing.md` — synchronisation temporelle & horodatage

## Références

- `docs/requirements/REQUIREMENTS.md` (précision, portée, simultanéité)
- `docs/technology-study/`
- `simulation/budget_liaison.ipynb`
