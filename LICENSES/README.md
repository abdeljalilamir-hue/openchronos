# Licences

Le projet OpenChronos mélange **trois types de contributions**, chacune sous sa propre licence. C'est une pratique courante en *open hardware*.

| Contenu | Dossier | Licence | Fichier |
|---|---|---|---|
| Logiciel & firmware | `firmware/`, `software/`, `tests/`, `simulation/` | **MIT** | `../LICENSE` |
| Matériel (schémas, PCB, BOM, CAO) | `hardware/`, `mechanical/` | **CERN-OHL-S v2** | `LICENSE-CERN-OHL-S-2.0.txt` *(à ajouter)* |
| Documentation & médias | `docs/`, `assets/` | **CC-BY-SA 4.0** | `LICENSE-CC-BY-SA-4.0.txt` *(à ajouter)* |

## Pourquoi ces licences ?

- **MIT** — permissive, maximise la réutilisation du code. Étudiants et futurs groupes peuvent repartir librement du code.
- **CERN-OHL-S v2** — la référence *open source* pour le matériel. La version **S** (*Strongly-reciprocal*) impose que toute réutilisation des schémas reste ouverte, ce qui protège l'open hardware du *lock-in*.
- **CC-BY-SA 4.0** — la doc reste libre d'utilisation avec attribution + partage à l'identique.

## À faire avant publication

1. Récupérer les textes officiels sur :
   - <https://ohwr.org/cern_ohl_s_v2.txt>
   - <https://creativecommons.org/licenses/by-sa/4.0/legalcode.txt>
2. Les déposer sous ce dossier avec les noms indiqués ci-dessus.
3. Mettre à jour le tableau et le README racine si les choix changent.

> ⚠️ Ces choix seront affinés avec l'encadrement (Mickaël BARON) avant publication officielle.
