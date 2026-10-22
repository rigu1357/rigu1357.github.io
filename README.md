# Personal website

Built with [Hugo](https://gohugo.io) and kept up to date with [folio](https://github.com/).

- Preview locally: `hugo server`, then open http://localhost:1313
- Content lives in `content/` (`projects/`, `research/`, `news/`). folio adds pages there when you publish.
- Change the look in `assets/css/style.css` and `layouts/`. Your name, tagline and links are in `hugo.toml`.
- Pushing to `main` deploys to GitHub Pages via `.github/workflows/hugo.yml`
  (in the repo's Settings → Pages, set Source to "GitHub Actions").
