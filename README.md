# classic-tips-home

Static homepage for `classic.tips`, currently hosted on GitHub Pages.

The site uses plain HTML, local CSS, and SVG. No installation or build step is required.

## Local preview

From the repository root, run:

```sh
python3 -m http.server 8080 --bind 127.0.0.1
```

Open `http://127.0.0.1:8080` in your browser.

## Updating the homepage

- Edit content and links in `index.html` and presentation in `styles.css`.
- Agent and AI are marked **Planned**. Their domain names are plain text until the websites launch. Add links and update their status when they are available.
- The blog, GitHub, Twitter / X, and email links retain the destinations from the original homepage.
- The footer year is static; update it when needed.
- Keep `CNAME` while using the existing GitHub Pages custom domain.

## Hosting on AWS later

These same static files can be deployed to AWS. Keep `index.html`, `styles.css`, and `favicon.svg` at the web root. For Amplify, use a manual static deployment or configure its Git build output directory to the directory containing `index.html`; no package installation is needed. Configure `classic.tips` as a custom domain in the selected hosting service before changing its DNS records.

