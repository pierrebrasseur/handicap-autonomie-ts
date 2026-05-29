# Handicap, autonomie et travail social — Quarto book

Livre académique [Quarto](https://quarto.org) qui rassemble le matériel pédagogique du module Bachelor en travail social *Handicap, autonomie et travail social* (HETS Genève), préparé pour la leçon probatoire HETS du 5 juin 2026.

## Prévisualiser en local

```bash
./quarto preview --to html
# ouvre http://localhost:port/ automatiquement
```

## Construire

```bash
./quarto render --to html   # HTML book
./quarto render --to pdf    # PDF (nécessite rsvg-convert + TinyTeX)
./quarto render             # tous les formats
```

Le site statique sort dans `_site/`.

## Déploiement

Le workflow `.github/workflows/quarto.yml` rend et publie automatiquement sur GitHub Pages à chaque push sur `main`.

## Structure

```
quarto_book/
├── _quarto.yml          # config du livre
├── index.qmd            # page de garde
├── chapters/            # 15 chapitres
├── appendices/          # 3 annexes
├── images/              # schémas SVG
├── references.bib       # BibTeX
├── theme-light.scss     # palette claire
└── theme-dark.scss      # palette sombre
```

## Licence

Contenu sous CC BY-NC-SA 4.0.
