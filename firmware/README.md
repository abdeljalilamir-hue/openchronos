# firmware/

Code embarqué (MCU).

## Organisation

- `transponder/` — firmware du transpondeur embarqué (émission). Contraintes : basse conso, simplicité.
- `receiver/` — firmware du récepteur + détection (réception, horodatage, sortie données).
- `common/` — code/protocole partagé (format trame, CRC, constantes).

## Choix d'IDE/SDK (à justifier via ADR)

Ex. PlatformIO, Zephyr, STM32Cube, ESP-IDF, Arduino, etc.
Favoriser un environnement **reproductible** (lockfile/manifest).
