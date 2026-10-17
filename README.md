# road2depth-site

Le site public de l'application Road2Depth, servi par GitHub Pages :
politique de confidentialité, assistance, mentions légales.

| Page | Chemin | Usage |
| --- | --- | --- |
| Accueil | `/` | URL marketing (facultative) |
| Politique de confidentialité | `/confidentialite/` | `PRIVACY_URL` de l'app, App Store Connect, Play Console |
| Assistance | `/assistance/` | URL d'assistance d'App Store Connect |
| Mentions légales | `/mentions-legales/` | obligation LCEN d'un site publié depuis la France |

## Règles

- **Les adresses ci-dessus sont écrites dans le binaire de l'app** : ne jamais
  renommer un dossier. Le jour d'un nom de domaine, ajouter un fichier `CNAME` :
  GitHub redirige alors l'ancienne adresse `github.io` vers le domaine.
- **Le site dit ce que fait l'app, rien de plus.** Toute évolution de l'app qui
  touche aux données (export, partage, sauvegarde, compte) se reporte dans
  `confidentialite/` dans le même mouvement — avec sa version et sa date.
- **Liens relatifs partout**, sauf dans `404.html` (servie à n'importe quelle
  profondeur) : le site doit fonctionner sous `/road2depth-site/` comme à la
  racine d'un domaine. Les chemins absolus de `404.html` sont donc à
  raccourcir (`/road2depth-site/` → `/`) le jour du domaine.
- **Aucune ressource tierce** : polices servies depuis `assets/fonts/`, aucun
  script, aucun cookie. La politique l'affirme du site.
- Avant de pousser : `grep -rln "À compléter" --include="*.html" .` doit être vide.

## Ressources

- `assets/logo.svg` — le tracé de `assets/images/depth-icon-navy.svg` du dépôt
  de l'app, recadré comme `Logo.tsx` (`viewBox 124 122 780 780`), en blanc.
- `assets/favicon.png` — copie de `assets/images/favicon.png` de l'app.
- `assets/fonts/` — Barlow et Barlow Semi Condensed (SIL OFL 1.1), copiées de
  `src/assets/fonts/` de l'app.
