# ijk37.github.io

Personal academic website for **Imran Jahid Khan** — served at [ijk37.com](https://ijk37.com).

## Stack
Plain HTML + CSS (no build step). Auto-deployed to GitHub Pages via `.github/workflows/static.yml` on every push to `main`.

## Structure
- `index.html` — the page content (edit text/sections here)
- `achievements.html` — scholarships, fellowships, and honors
- `assets/style.css` — all styling (colors live in the `:root` variables at the top)
- `assets/profile.jpg` — profile photo
- `assets/IJK_CV_site.pdf` — public CV linked from the sidebar (no GPA/CGPA)
- `cv-src/` — editable CV source; retained in the repository but not published
- `CNAME` — custom domain (`ijk37.com`)
- `.github/workflows/static.yml` — publishes only the public website files to GitHub Pages

## Editing
Update biography, research, publications, news, and conference activity in `index.html`.
Update scholarships and honors in `achievements.html`. Replace `assets/IJK_CV_site.pdf` whenever the CV changes.

Both CV versions share `cv-src/cv_common.tex`. Compile `cv_site.tex` and `cv_academic.tex`
from the `cv-src` directory with `pdflatex` twice each. The private academic wrapper adds
GPA/CGPA and the phone number; all other content and formatting are shared. Copy the site build to
`assets/IJK_CV_site.pdf` and `IJK_CV_site.pdf`, and the academic build to `IJK_CV_Academic.pdf`.
The academic wrapper and PDF remain git-ignored and are not deployed.

Publication buttons should only be added when their PDF, DOI, or BibTeX destination is available; do not use placeholder links.

## Local preview
Open `index.html` directly in a browser, or run a static server:
```
python -m http.server 8000
```

Then visit `http://localhost:8000`.
