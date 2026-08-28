# Portfolio de Melvyn — Guide d'utilisation

Site portfolio one-page de Melvyn Jean-Pierre, apprenti pâtissier.

## Contenu du ZIP

```
index.html          — le site complet (textes, styles et animations intégrés)
images/
├── melvyn.jpg          — portrait affiché dans l'accueil
├── flan.jpg            — photo du flan marbré chocolat-vanille
├── viennoiseries.jpg   — photo des croissants et pains au chocolat
└── makrouts.jpg        — photo des makrouts aux dattes
README.md           — ce guide
```

⚠️ **Important** : le fichier `index.html` et le dossier `images/` doivent toujours rester ensemble, au même niveau. Si vous déplacez `index.html` sans le dossier `images/`, les photos ne s'afficheront plus.

## Ouvrir le site

Double-cliquez sur `index.html` : il s'ouvre dans votre navigateur.

---

## Héberger sur GitHub Pages (gratuit, étape par étape)

1. Créez un compte sur [github.com](https://github.com) si ce n'est pas déjà fait.
2. Cliquez sur **New repository** (nouveau dépôt), nommez-le par exemple `portfolio-melvyn`, laissez-le **Public**, puis validez.
3. Sur la page du dépôt, cliquez sur **uploading an existing file**.
4. Glissez-déposez **le contenu dézippé** : `index.html` ET le dossier `images/` (avec ses 4 photos). Cliquez sur **Commit changes**.
5. Allez dans **Settings → Pages**.
6. Sous **Source**, choisissez la branche `main` et le dossier `/ (root)`, puis **Save**.
7. Patientez 1 à 2 minutes : votre site est en ligne à l'adresse `https://votre-pseudo.github.io/portfolio-melvyn/`.

Pour toute mise à jour ultérieure : retournez sur le dépôt, supprimez l'ancien fichier et téléversez le nouveau (ou utilisez **Add file → Upload files**).

---

## Remplacer une photo existante

C'est l'opération la plus simple :

1. Préparez votre nouvelle photo (JPG, environ 1200 pixels de large maximum).
2. Renommez-la exactement comme le fichier à remplacer (`melvyn.jpg`, `flan.jpg`, `viennoiseries.jpg` ou `makrouts.jpg`).
3. Remplacez le fichier dans le dossier `images/`.
4. C'est tout — le site affichera la nouvelle photo, sans toucher au code.

---

## Ajouter une nouvelle recette avec photo

Ouvrez `index.html` avec un éditeur de texte (Bloc-notes, Notepad++, VS Code…).

### Étape 1 — Ajouter la photo

Placez votre photo dans le dossier `images/`, par exemple `images/tarte-citron.jpg`.

### Étape 2 — Dupliquer une fiche

1. Dans `index.html`, cherchez (Ctrl+F) `Carnet de progression`.
2. Repérez les blocs qui commencent par `<article class="card fade-in">` et se terminent par `</article>`.
3. Copiez un bloc complet (du `<article` au `</article>` inclus) et collez-le juste après le dernier `</article>`, toujours à l'intérieur de `<div class="cards">`.

### Étape 3 — Personnaliser la fiche

Dans le bloc copié, modifiez :

1. **La photo** : dans `<img class="card-img" src="images/flan.jpg" alt="...">`, remplacez `flan.jpg` par le nom de votre fichier (ex. `tarte-citron.jpg`) et adaptez le texte `alt` qui décrit la photo (important pour l'accessibilité).
2. **Le badge** : le texte dans `<span class="badge">…</span>` (ex. `Classique revisité`, `Viennoiserie`, `Entremets`…).
3. **Le titre** : le texte dans `<h3>…</h3>`.
4. **L'objectif** : la phrase dans `<p class="objectif">…</p>`.
5. **Les techniques** : ajoutez ou supprimez des lignes `<li>…</li>` dans la liste `<ul>`.
6. **Le résultat** : le texte dans `<p class="resultat">…</p>` — restez honnête, c'est la force du site !
7. **Ce que j'en retiens** : le texte dans `<div class="retiens">…</div>`.

### Étape 4 — Vérifier et publier

1. Enregistrez (Ctrl+S) et ouvrez `index.html` dans votre navigateur : la nouvelle fiche apparaît.
2. Pour mettre à jour le site en ligne, renvoyez `index.html` et le dossier `images/` complet sur GitHub.

---

## Modifier les textes

Tous les textes sont en clair dans `index.html` : cherchez la phrase à changer avec Ctrl+F, modifiez-la, enregistrez.
