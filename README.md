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

- Le bouton « Rejoindre les tests » attend le **lien public TestFlight**
  (`https://testflight.apple.com/join/XXXXXXXX`). Il est actuellement
  désactivé, avec l'adresse e-mail en repli. Chercher le commentaire
  `REMPLACER` dans `index.html`.
- `marc@gofree.fr` est une redirection OVH vers la boîte personnelle.
  Nom volontairement non générique : `contact@` et `info@` sont attaqués au
  dictionnaire par les robots, sans même avoir à les trouver sur une page.

## Développement

```sh
python3 -m http.server 8911
```
