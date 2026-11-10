# GreenholdDemo

The public demo of the Greenhold Manager at https://demo.greenhold.eu: a simple tour of the main
pages with made-up data, so a visitor sees how Greenhold looks and works.

- `site/` is the published site: static HTML, CSS and fonts only, nothing loaded from another site.
  It is made on the build computer from Greenhold's Mock Testing and committed here; it is not
  built in CI.
- `.github/workflows/deploy.yml` checks the site (index page, CNAME, nothing loaded from elsewhere,
  every local link points at a file) and publishes `site/` to GitHub Pages on a push to `main`.
  A pull request is checked only.
- The demo is updated only when the owner says so at a release.
