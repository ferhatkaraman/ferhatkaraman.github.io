# Quarto CV (HTML + PDF) — Ferhat Karaman

This is a clean, professional CV you can edit in one place and render to:

- **HTML** (great for GitHub Pages)
- **PDF** (for job applications)

## Quick start

1. Install Quarto: https://quarto.org/docs/get-started/
2. In this folder, run:

```bash
quarto render cv.qmd
```

It will create `_site/` (HTML) and `cv.pdf`.

## Deploy to GitHub Pages (fast)

1. Create a repo (e.g., `cv`)
2. Put these files in the repo root.
3. In **GitHub → Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/docs` **OR** use the built-in Quarto publishing workflow below.

### Option A: Use /docs (no Actions)

- Render HTML to `docs/` instead of `_site/` by adding to the YAML:

```yaml
project:
  output-dir: docs
```

Then commit and push.

### Option B: GitHub Actions (recommended)

Use Quarto’s official Pages workflow:
https://quarto.org/docs/publishing/github-pages.html

## Editing tips

- Keep the **core content** in `cv.qmd`.
- Add new items under the relevant headings.
- For publications, consider keeping them in a `publications.bib` file later (optional).
