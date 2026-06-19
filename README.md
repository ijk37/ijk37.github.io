# ijk37.github.io

Personal academic website for **Imran Jahid Khan** — served at [ijk37.com](https://ijk37.com).

## Stack
Plain HTML + CSS (no build step). Auto-deployed to GitHub Pages via `.github/workflows/static.yml` on every push to `main`.

## Structure
- `index.html` — the page content (edit text/sections here)
- `assets/style.css` — all styling (colors live in the `:root` variables at the top)
- `assets/profile.svg` — placeholder avatar; replace with a real photo (`assets/profile.jpg`) and update the `<img src>` in `index.html`
- `assets/cv.pdf` — add your CV here (the sidebar link points to it)
- `CNAME` — custom domain (`ijk37.com`)

## Editing
Search `index.html` for `TODO:` comments — those mark the spots to personalize (affiliation, profile links, publications, news).

## Local preview
Open `index.html` directly in a browser, or run a static server:
```
python -m http.server 8000
```
