# VINE — Project Page

Template project page for **VINE**. Deployed at **`/vine`** (GitHub Pages project site).

## Local Preview

From this directory:

```bash
python -m http.server 8000
```

Open **http://localhost:8000** — note that asset paths use `/vine/`, so for full local preview either:

- serve from a parent setup that maps `/vine/` to this folder, or
- temporarily change paths from `/vine/...` to relative (`style.css`, `images/...`).

## Page Structure

Single-page layout (template sections):

- **Abstract** — abstract + teaser figure
- **Method** — overview, visualization grid, highlights, steps
- **Experiments** — task demos, results, training curves, ablations
- **Qualitative Results** — single video block
- **Robustness** — scrollable + single video blocks
- **Generalization** — ID/OOD demos and figures
- **Analysis** — ablation table + diagnostic figures
- **Citation** — BibTeX

## What to Edit

| Where | What |
|-------|------|
| **Title / authors** | Top of `index.html` |
| **Action links** | Paper, Code URLs |
| **Section text** | Replace `(TBD)` placeholders |
| **images/** | `teaser.png`, `results.png`, etc. |
| **videos/** | `demo_*.mp4`, `qualitative.mp4`, etc. |
| **BibTeX** | Citation block at bottom |

All asset paths are prefixed with **`/vine/`** for GitHub Pages deployment.

## GitHub Pages (`/vine`)

1. Push this folder as repo **`vine`** (or configure Pages to serve from `/vine`).
2. **Settings → Pages** → deploy from `main`, root `/`.
3. Live URL: **https://&lt;username&gt;.github.io/vine/**

## Repo Layout

```
├── index.html
├── style.css
├── README.md
├── images/         # figures (add your own)
└── videos/         # demo videos (add your own)
```
