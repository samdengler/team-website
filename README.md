# Developer Advocacy Team Website

This repository contains a static landing page for the DevRel Collective developer advocacy team. It is designed to be embedded in Confluence via HTML and CSS macros while remaining easy to preview locally.

## Structure

- `index.html` – Single-page site with all content for the landing experience.
- `assets/css/styles.css` – External stylesheet referenced by the HTML page.

## Local preview

You can use any static file server. For example, with Python installed:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser.

## Deployment to Confluence

1. Upload `assets/css/styles.css` to a Confluence space or static asset host reachable by Confluence.
2. Embed `index.html` inside an HTML macro, updating the `<link rel="stylesheet">` path if needed to point to the hosted CSS file.
3. Remove the `<script>` block if dynamic year updates are not supported by the hosting environment.
