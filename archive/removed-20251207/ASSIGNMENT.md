Design Style Vibe Coding — Quick Assignment Guide

This repository contains a starter site that demonstrates a single design language (Material/Pixel). Use the files and template here to create one site per design style for the class assignment.

What you must deliver
- A public URL (GitHub Pages or similar) to a site that demonstrates a single design style and includes a short research/history write-up.
- Add your site under `docs/<style-name>/index.html` and link it from `docs/gallery.html`.

How to scaffold a new style site
1. Copy `docs/style-template.html` to `docs/<style-name>/index.html`.
2. Replace `STYLE NAME` and the placeholder text with your research, 3+ references, and demo components.
3. Use images in `docs/assets/` or add new SVGs to `docs/assets/`.
4. Link back to `docs/gallery.html` (and optionally to other students' pages).

Local preview
From the repo root run:
```bash
cd docs
python3 -m http.server 8000
# then open http://localhost:8000/gallery.html
```

Submission
- Submit the public URL to your instructor (the `docs/<style-name>/index.html` page deployed via GitHub Pages or raw URL).
- Make sure `docs/gallery.html` includes a link to your page.

Notes
- Preserve accessibility behaviors in the inline scripts (reduced-motion, ripple sizing).
- Prefer using the provided CSS utilities instead of creating unnecessary global rules.
