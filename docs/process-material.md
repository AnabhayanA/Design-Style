# Process Notes — Material Submission

This document records the steps taken to convert the starter site into a Material-style submission.

Work completed:
- Audited the repo against a Material Design authenticity checklist (`docs/material-audit.md`).
- Added CSS tokens (`:root`) for spacing (`--unit`), colors, shadows, and motion variables in `docs/style.css`.
- Normalized elevation (`.elevation-*`) to use shadow tokens and adjusted radii to Material 4px where appropriate.
- Shortened ripple animation and DOM removal timing to match Material durations.
- Added a visible `Material Palette` demo section to `docs/index.html` showing primary/secondary colors.
- Added motion/stagger utilities and updated IntersectionObserver scripts to support staggered reveals.
- Added a GitHub Actions workflow to publish `docs/` to GitHub Pages automatically.

Next recommended steps (optional but recommended before final submission):
- Add 4–6 optimized demo images (PNG or compressed JPEG) to `docs/assets/` for richer component examples.
- Capture 5–10 screenshots of the site in mobile/tablet/desktop sizes and add them to `docs/process-material.md`.
- Run Lighthouse and adjust for performance/accessibility (image sizes, font loading, unused CSS).
- Double-check color contrast with the accessibility tool and adjust tints if needed.

AI collaboration notes
- Iterated with an AI assistant to: add tokens, standardize motion, build palette section, and scaffold research/process docs.
- Files created/updated: `docs/material-audit.md`, `docs/style.css`, `docs/index.html`, `docs/assests`, `.github/workflows/deploy-pages.yml`, `research/material/references.md`, `docs/process-material.md`.
