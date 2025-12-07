# Design-Style — Material Submission

This repository contains a Material-style demo in `docs/` suitable for the Design Style Vibe Coding assignment.

Local preview
- Start a static server from the `docs/` folder and open the site in your browser:

```bash
cd /home/anabhayan/Design-Style/docs
python3 -m http.server 8000
# open http://localhost:8000/index.html (or /gallery.html)
```

Automatic deployment to GitHub Pages
- I added a GitHub Actions workflow at `.github/workflows/deploy-pages.yml` that automatically publishes the `docs/` folder to the `gh-pages` branch whenever you push to `main`.

How it works
1. Commit & push your changes to `main`.
2. The workflow runs, pushes a `gh-pages` branch containing the built `docs/` files.
3. GitHub Pages serves the site from the `gh-pages` branch — your site URL will be:
   `https://<your-username>.github.io/<repo-name>/`

Notes & post-deploy steps
- If GitHub Pages does not appear immediately, open the repository Settings → Pages and ensure the source is `gh-pages` branch (root). The Pages status UI will show the live URL once deployed.
- If you prefer to serve from the `docs/` folder (without `gh-pages`), you can also set Pages source to `main` → `docs/` in Settings.

Manual publish (alternative)
- If you prefer not to use Actions, you can publish manually:

```bash
# create a branch with the docs site
git checkout --orphan gh-pages
git --work-tree=docs add --all
git --work-tree=docs commit -m "Publish docs to GitHub Pages"
git push origin gh-pages --force
git checkout main
```

Questions or want me to deploy and verify the URL? I can run through the push/test steps with you.
