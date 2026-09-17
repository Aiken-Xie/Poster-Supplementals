# DRBX Poster Supplementals

This repository contains the public, mobile-first companion site for the DRBX
research poster. It is intentionally separate from the DRBX source repository.

## Published site

When GitHub Pages is enabled and the deployment workflow completes, the site
will be available at:

<https://aiken-xie.github.io/Poster-Supplementals/>

## Layout

- `site/` is the complete public website.
- `site/assets/movies/` will hold the final web-optimized MP4 animations.
- `site/assets/previews/` will hold the small static images shown before a
  visitor chooses to play a movie.
- `site/assets/stills/` will hold non-moving scientific-figure alternatives.
- `site/assets/poster/` will hold the final downloadable poster PDF.
- `.github/workflows/deploy-pages.yml` deploys only `site/` to GitHub Pages.

Do not add raw render outputs, simulation data, or archival-quality movies to
this repository. Keep those in research storage or a release archive; add only
the compact files intended for the public page.

## Publishing

1. In the repository on GitHub, open **Settings → Pages**.
2. Under **Build and deployment**, choose **GitHub Actions**.
3. Push to `main`. The deployment workflow publishes `site/` automatically.

The root page is the QR-code destination. Keep its URL stable; update its
contents rather than renaming or replacing the repository.
