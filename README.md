# Mow & Flow

Static single-page marketing site for Mow & Flow — Sydney-based luxury lawn care and exterior home finishes.

## Stack

Plain HTML, CSS, and a touch of vanilla JS. No build step. Google Fonts (Fraunces, Inter).

## Local preview

Open `index.html` in a browser, or serve the directory:

```sh
python -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Pushed to `main` and deployed to GitHub Pages via `.github/workflows/deploy.yml`.

The primary site is served from the repository root. The alternate concept is deployed from `alternative/` and is available at `/alternative/` on GitHub Pages.

## Files

- `index.html` — markup
- `styles.css` — all styles
- `main.js` — sticky-header state and mobile nav
- `favicon.svg` — italic ampersand mark
- `assets/` — images (placeholders until real photography is dropped in)
- `docs/SPEC.md` — site specification
- `alternative/` — alternate site concept deployed as a subfolder
