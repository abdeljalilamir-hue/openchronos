# Informations issues du rapport "Problématique, Besoins et attentes de l'entreprise"

**Document source** : `C:\Users\PC\Downloads\Rapport Projet Innovation  Problématique, Besoins et attentes de l’entreprise.docx`

## 1. Contexte & Équipe
- **Entreprise** : ISAE-ENSMA — Laboratoire LIAS
- **Tuteur ECC** : Mr Chafik EL KIHAL
- **Tuteur Entreprise** : Mr Mickaël BARON
- **Groupe** : 35
- **Salle BootCamp** : A107

## 2. Problématique
> *Comment concevoir une solution de chronométrage open source, fiable, accessible et reproductible pour des véhicules de taille réelle, tout en garantissant une identification précise des concurrents et une évolution possible du système ?*

## 3. Compréhension du besoin
Il s'agit de concevoir un **système de chronométrage sportif par transpondeur actif** pour des sports motorisés (moto, karting, etc.).

Le dispositif devra être **couplé à un logiciel** avec une **expérience utilisateur (UX)** intéressante :
- Consultation des résultats, classements, compétitions
- Utilisation sur **PC et téléphone**

## 4. Public visé
**Petits clubs et clubs amateurs**. Le frein principal est le **prix élevé de l'infrastructure de chronométrage** (limite entraînements et compétitions, ralentit l'évolution et la progression des membres).

**Exigence** : solution **abordable** tout en garantissant un **niveau convenable de performance** (identification précise des concurrents, prise de temps précise).

## 5. Attentes de l'entreprise (LIAS / M. Baron)
L'entreprise **n'attend pas** un prototype fonctionnel pour la partie hardware.

Elle attend **une étude rigoureuse de toutes les étapes avant le prototypage**, comprenant :

1. **Compréhension de la problématique et du besoin**
2. **Étude de l'état de l'art**
3. **Justification de la solution choisie**
4. **Business Model**
5. **Étude des matériaux nécessaires à la fabrication du hardware**
6. **Un logiciel avec une bonne UX**
7. **Étude du marché et des coûts de fabrication**
8. **Simulation et modélisation du système retenu**
9. **Documentation permettant la réalisation du prototype**
10. **Protocole de test et validation de la solution**

## 6. Étude technique demandée
En complément de la partie gestion de projet :
- Étude technique de la solution
- Son **électronique**
- La **transmission du signal** et son **traitement**

## 7. Impact sur la structure du repo

Le sujet initial (fichier PDF) demandait surtout la **conception** (architecture, technologies, justification, schémas, coûts, tests). Ce rapport précise fortement les attendus en **étude/amont** (état de l'art, business model, marché, coûts, simulation/modélisation, UX logicielle).

**Conclusion** : la structure complète que l'on a créée est **très bien adaptée** (couvre déjà docs, simulation, hardware/firmware/software, validation). Quelques compléments recommandés pour coller parfaitement aux attentes :

| À ajouter | Où | Pourquoi |
|---|---|---|
| `docs/market-study/` | Nouveau dossier | Étude du marché + Business Model (points 4 et 7) |
| `docs/business-model/` ou `docs/market-study/business-model.md` | À créer | Point Business Model explicite |
| `docs/state-of-art/` | Peut fusionner avec `docs/technology-study/` | État de l'art demandé (point 2). On peut renommer ou ajouter un `etat-de-lart.md` dedans |
| `docs/materials/` | Nouveau dossier | Étude matériaux hardware (point 5) |
| Mettre l'accent UX | `docs/software/ux.md` | Demande UX explicite (point 6) |

**Recommandation pratique** : **ne pas tout casser**. On peut enrichir les dossiers existants sans renommer tout (ex. ajouter `etat-de-lart.md` dans `docs/technology-study/`, créer `docs/market-study/` avec `market.md` + `business-model.md`, `docs/materials/`).

La structure reste **compatible**, juste enrichie pour mieux répondre aux livrables attendus par le groupe + encadrement.