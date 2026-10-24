# Mosaïk

Mosaïk est un puzzle de tuiles : place les pièces, complète les lignes et enchaîne les combos.

Le jeu tient dans un seul fichier, `index.html`, sans installation ni serveur à préparer. Tout fonctionne directement dans le navigateur, sur ordinateur comme sur téléphone.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | Le jeu complet. |
| `manifest.webmanifest` | Permet d'ajouter le jeu à l'écran d'accueil du téléphone, comme une app. |
| `sw.js` | Permet de rejouer sans connexion après une première visite. |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | Les icônes du jeu. |
| `.nojekyll` | Demande à GitHub Pages de publier les fichiers tels quels. |
| `confidentialite.html` | La politique de confidentialité. Son adresse sert aussi pour l'App Store. |
| `support.html` | La page d'assistance (mets ton adresse e-mail dedans). Son adresse sert aussi pour l'App Store. |
| `OFL-Bricolage.txt` | La licence libre de la police des titres, intégrée au jeu. |

## Mettre le jeu en ligne avec GitHub Pages

1. Sur github.com, crée un nouveau dépôt **public**, par exemple `mosaik`.
2. Dans le dépôt, clique sur **Add file → Upload files**.
3. Glisse **tous les fichiers de ce dossier**, y compris `.nojekyll`. Si ce fichier ne s'affiche pas sur ton ordinateur, ce n'est pas grave : il n'est pas indispensable.
4. Clique sur **Commit changes**.
5. Va dans **Settings → Pages**.
6. Dans « Build and deployment », choisis la source **Deploy from a branch**, puis la branche **main** et le dossier **/ (root)**. Clique sur **Save**.
7. Attends une à deux minutes. Ton jeu est alors en ligne à l'adresse `https://TON-PSEUDO.github.io/mosaik/`.

## Jouer sur iPhone comme une app

1. Ouvre l'adresse du jeu dans **Safari**.
2. Touche le bouton **Partager**, puis **Sur l'écran d'accueil**.
3. Mosaïk apparaît avec son icône. Il s'ouvre en plein écran et marche aussi sans connexion après une première partie.

## Mettre à jour le jeu

Remplace `index.html` dans le dépôt par la nouvelle version, avec **Add file → Upload files** puis **Commit changes**. Les joueurs reçoivent la mise à jour à leur prochaine ouverture du jeu.

## Bon à savoir

- **Sauvegarde :** la progression (score, pièces, styles achetés) est enregistrée dans le navigateur de chaque joueur. Elle n'est pas partagée entre deux appareils, et elle est perdue si le joueur efface les données de son navigateur.
- **Pubs et achats :** dans cette version web, les pubs et les achats sont simulés. Aucune vraie pub ne s'affiche et aucun paiement n'est demandé. Les vraies pubs et les vrais achats passent par l'app iOS (projet Xcode).
