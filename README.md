# Jeongsik Park — Personal Website

Personal academic website, served as plain static files (no build step) at
<https://lucasjeongsikpark.github.io/>.

## Structure

- `index.html` — landing page with links to each section
- `sections/` — resume, education, publications, professional service, awards, contact, news, miscellaneous
- `projects/` — unlisted project pages (`noindex`, reachable only by direct URL)
- `assets/css/section.css` — shared styles for section pages
- `assets/css/project.css` — shared styles for project pages
- `assets/pdfs/` — project report PDFs linked from project pages
- `style.css` + `fonts/` — LaTeX-style base theme (derived from [latex.css](https://github.com/vincentdoerig/latex-css), MIT) with local customizations
- `data/` — archived CV/resume and report PDFs (not linked from any page)

## Local preview

```bash
npm start
```

Then open <http://localhost:8000>. Any static file server works; there is no build step.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which uploads the repository
as-is to GitHub Pages (Settings → Pages → Source must be set to "GitHub Actions").

## Upstream leftovers

This repo started as a fork of [latex.css](https://github.com/vincentdoerig/latex-css).
The following files are unused upstream artifacts kept for now; they are safe to delete later:
`CHANGELOG.md`, `elements.html`, `languages.html`, `lang/`, `vite.config.js`, `prism/`, `projcts/`.

## Acknowledgements

The base stylesheet (`style.css`, `fonts/`) is derived from
[latex.css](https://github.com/vincentdoerig/latex-css) by Vincent Dörig,
used under the [MIT License](LICENSE).
