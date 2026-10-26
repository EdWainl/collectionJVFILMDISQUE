# Mes collections

Tableau de bord de ma collection de films, séries et disques (page unique, sans dépendance externe).

## Publier sur GitHub Pages (sans ligne de commande)

1. Connectez-vous sur https://github.com puis **New repository** (le « + » en haut à droite).
   Donnez un nom (par exemple `mes-collections`), laissez **Public**, cliquez **Create repository**.
2. Dans le dépôt vide : **uploading an existing file** (ou Add file > Upload files).
   Glissez le contenu du dossier : `index.html`, `robots.txt`, `README.md` (et `.nojekyll` si votre système vous le permet : il est facultatif).
   Cliquez **Commit changes**.
3. **Settings** > **Pages** > section *Build and deployment* :
   Source = **Deploy from a branch**, Branch = **main**, dossier **/ (root)**, puis **Save**.
4. Attendez 1 à 2 minutes. L'adresse apparaît en haut de la page Pages :
   `https://VOTRE-PSEUDO.github.io/mes-collections/`

Liens directs vers chaque collection :
- `https://VOTRE-PSEUDO.github.io/mes-collections/#films`
- `https://VOTRE-PSEUDO.github.io/mes-collections/#disques`

## Publier en ligne de commande

```bash
cd MesCollections_GitHubPages
git init -b main
git add .
git commit -m "Mes collections"
git remote add origin https://github.com/VOTRE-PSEUDO/mes-collections.git
git push -u origin main
```
Puis réglez Settings > Pages comme à l'étape 3.

## Mettre à jour
Remplacez `index.html` par la nouvelle version (même nom) et validez (commit) : le site se met à jour en 1 à 2 minutes.

## Confidentialité : à lire
Les données de la collection sont **contenues dans index.html**. Sur un compte GitHub gratuit, un site GitHub Pages est **public** : toute personne qui connaît l'adresse peut voir la collection complète, et le code source du dépôt est lisible. Les balises `noindex` et `robots.txt` demandent aux moteurs de recherche de ne pas référencer la page, mais ne la protègent pas.
