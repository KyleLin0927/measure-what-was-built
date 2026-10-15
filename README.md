# Measure What Was Built — project page (GitHub Pages)

Self-contained static site: `index.html` + `assets/` (JPEG renders). No build step, no external dependency except Google Fonts (optional; the page falls back to system fonts).

## Publish on GitHub Pages (three steps)

1. Create a new repository (public, e.g. `measure-what-was-built`).
2. Put the contents of this directory at the repository root (or inside `docs/`): `index.html`, `assets/`, `.nojekyll`.
3. On GitHub: **Settings › Pages › Build and deployment › Source = Deploy from a branch**, pick the branch (`main`) and the folder (`/ (root)` or `/docs`), save. The page appears at `https://<user>.github.io/<repo>/` after a minute.

`.nojekyll` tells Pages to serve the files as-is (no Jekyll processing).

## Preview locally

```
cd <this directory>
python3 -m http.server 8000
```

then open http://localhost:8000/ in a browser.
