# gofree.fr

Site vitrine de l'application **GO FREE** — GPS tout-terrain pour
moto et 4×4 en France, bientôt camping-car.

Statique : HTML + CSS, aucune dépendance, aucune étape de build. Polices
auto-hébergées. Publié par GitHub Pages depuis `main`.

## Structure

```
index.html      la page
styles.css      le monde visuel (voir ../DESIGN.md)
fonts.css       @font-face vers les fichiers locaux
fonts/          Rajdhani + Barlow, sous-ensembles latin (124 Ko)
img/            captures réelles de l'application
```

## À remplacer

- Le **lien public TestFlight** est en place : son code vit dans
  `data-testflight` (`index.html`), et l'URL complète est recomposée par le
  script. Pour le changer, remplacer les huit caractères qui suivent `/join/`.
  Si l'attribut est vidé, le bouton retombe sur l'adresse e-mail.
- Le bloc TestFlight ne sort que sur iPhone : sur Android, le script retire
  `[data-plateforme="ios"]` du document et affiche le bloc Android à la place
  (« la version Android arrive », même adresse e-mail). Le lien d'invitation
  n'est donc jamais composé sur un appareil Android.
- `marc@gofree.fr` est une redirection OVH vers la boîte personnelle.
  Nom volontairement non générique : `contact@` et `info@` sont attaqués au
  dictionnaire par les robots, sans même avoir à les trouver sur une page.

## Développement

```sh
python3 -m http.server 8911
```
