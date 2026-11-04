# ChipletNet 2027 Workshop website

Static single-page site served by GitHub Pages: `index.html` + `css/style.css`, no build step and no JavaScript.

## Editing

- Content lives in `index.html`. The Attendees and Program sections contain commented-out examples
  (attendee list, per-day program table) to copy from when the TBD placeholders are replaced.
- Styles: `css/style.css`. Colors are set at the top (`--brand` navy, `--accent` red).
- Images: organizer photos in `img/organizers/`, sponsor logos in `img/sponsors/`, talk slides (PDF) in `slides/`.
- Logo: `img/logo.svg` (for light backgrounds), `img/logo-dark.svg` (for dark backgrounds, used in the banner),
  `img/logo-icon.svg` (icon only, used as the favicon).

Preview locally:

    python3 -m http.server 8000   # then open http://localhost:8000

## Deploying to GitHub Pages

1. Create a repo, e.g. `<org>/chipletnet2027` (served at `https://<org>.github.io/chipletnet2027/`),
   or `<org>/<org>.github.io` to serve it at the root.
2. Push this directory to the `main` branch.
3. In the repo: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.

`.nojekyll` disables Jekyll processing, so files are served as-is.
