## Repo créé localement

Le dépôt est prêt sur votre PC :

**Chemin :** `C:\Users\PC\OneDrive\Documents\Projet par défaut\openchronos`

**Contenu :** structure complète, README, LICENCE, CONTRIBUTING, CHANGELOG, .gitignore + squelettes pour docs/hardware/firmware/software/mechanical/simulation/tests/assets + ADR + cahier des besoins + protocole de test + BOM vide.

**Git :** `git init`, branche `main`, commit initial (`27e962a`) fait.

## Créer le repo GitHub & pousser

Comme vous n'avez pas de token, faites ça en ligne + terminal.

### 1) Créer le repo sur github.com

1. Allez sur [github.com](https://github.com) → Connectez-vous → `+` (haut droite) → `New repository`
2. **Repository name :** `openchronos`
3. **Visibility :** `Public`
4. **NE PAS** cocher "Add a README / .gitignore / license" (déjà présents)
5. Cliquer `Create repository`

### 2) Pousser le dépôt local

Ouvrez un terminal **PowerShell** dans ce dossier :

```powershell
cd "C:\Users\PC\OneDrive\Documents\Projet par défaut\openchronos"
```

Ajoutez l'URL distante (remplacez `VOTRE_LOGIN` par votre pseudo GitHub) :

```powershell
git remote add origin https://github.com/VOTRE_LOGIN/openchronos.git
git push -u origin main
```

Si Git vous demande vos identifiants, utilisez votre **pseudo GitHub** + un **Personal Access Token** (Settings → Developer settings → Tokens → Fine-grained tokens ou classic) comme mot de passe. Ou mieux, utilisez `gh` ou SSH.

### Alternative avec SSH

Si vous avez déjà une clé SSH configurée :

```powershell
git remote add origin git@github.com:VOTRE_LOGIN/openchronos.git
git push -u origin main
```

## À faire juste après

1. Copier le PDF du sujet dans `docs/subject/` si vous voulez le versionner.
2. Commencer par `docs/requirements/REQUIREMENTS.md` (chiffrer vitesse/précision/portée).
3. Ouvrir `docs/architecture/adr/TEMPLATE.md` pour créer le premier ADR.

Quand vous avez créé le repo et poussé, dites-moi l'URL — je peux générer le premier ADR ou le document requirements avec les ordres de grandeur directement dedans.