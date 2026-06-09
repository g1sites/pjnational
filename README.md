# pjnational.com

Static export of [pjnational.com](https://pjnational.com), deployed to Cloudflare Pages.

## Editing workflow

1. Edit the site in [Brizy Cloud](https://www.brizy.io/) (source of truth for content)
2. Export the site to HTML
3. Re-commit the export to this repo's `main` branch
4. Cloudflare Pages auto-deploys on push

## Structure

- `index.html` — homepage (single-page site)
- `b-cloud.becdn.net/` — Brizy editor CSS/JS (vendored from BunnyCDN)
- `cloud-1de12d.becdn.net/` — site media (logo, etc.)
- `fonts.bunny.net/` — fonts and bootstrap assets

The contact form posts to JotForm (`form.jotform.com/g1preet/webcontact-pjn`) — do not change that URL.

## Local preview

```
python3 -m http.server 8000
# open http://localhost:8000
```
