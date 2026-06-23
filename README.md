# ALOE — Project Page

Project page for **ALOE: Action-Level Off-Policy Evaluation for Vision-Language-Action Model Post-Training**. The paper is available on arXiv; you can link to this page from the paper.

## Local Preview

From the repo root, run a static server:

```bash
# Python 3
python -m http.server 8000

# or
npx serve .
```

Then open **http://localhost:8000** in your browser.

## Page Structure

Single-page layout with no pagination:

- **Abstract** — Paper abstract
- **Overview Figure** — Teaser/process figure under the abstract
- **Method** — Mixed replay intuition, behavior-policy value mismatch, ALOE's action-value definition, Q-chunking, pessimistic ensemble, and advantage-weighted policy extraction
- **Task Demos** — Four task videos (phone, cloth, pick-and-place, phone assembly)
- **Continuous Operation** — Phone packing 21-trial video
- **Final Results** — four-task success-rate and policy-improvement figures
- **Robustness** — Phone disturb ×3 + cloth disturb ×1
- **OOD Generalization** — Unseen object pick videos
- **Critic Analysis** — Critic ablations, calibration, action ranking, and component analysis
- **Contributions** — Bullet points
- **Citation** — BibTeX with the arXiv ID

## What to Edit

| Where | What |
|-------|------|
| **Action links** (top) | Set **Paper (PDF)** to your arXiv URL; **Code** and **Video** to repo/demo links |
| **Authors** | Update `href` to personal/Google Scholar pages if desired |
| **BibTeX** | Keep authors and arXiv metadata aligned with the latest paper source |
| **images/** | Keep generated paper figures such as `final_result.pdf`, `policy_improvement.pdf`, and `throughput_generalization.pdf` in sync |

Videos in `videos/` and images in `images/` are used as-is; paths are in `index.html`.

## GitHub Pages

1. Push this repo to GitHub (e.g. **Rooshy-yang/aloe**).
2. Go to **Settings → Pages**.
3. **Source**: Deploy from a branch.
4. **Branch**: `main`, **Folder**: `/ (root)`.
5. Save. After a minute or two, the site will be at:
   - **https://rooshy-yang.github.io/aloe/**

## Link in Your Paper

In the paper, point to the project page:

> Project page: https://rooshy-yang.github.io/aloe/

## Repo Layout

```
├── index.html      # Main page
├── style.css       # Styles
├── README.md       # This file
├── images/         # teaser.png, Q_value2_cropped.png, final result figures
└── videos/         # Task demos, robustness, OOD, phone_success_rate, etc.
```

After editing, commit and push to update the live page.
