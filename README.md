# sonder-site

Static landing page for [Sonder](https://github.com/amayabdaniel/sonder-clients) — pure HTML + CSS, deployed to GitHub Pages.

## Layout

- `index.html` — hero + how it works + privacy + install grid
- `privacy.html` — full privacy policy (mirrors `sonder-clients/PRIVACY.md`)
- `consent.html` — consent notice + jurisdictional guidance
- `style.css` — single stylesheet, dark/light auto via `prefers-color-scheme`
- `.github/workflows/pages.yml` — Pages deploy on push to `main`

## Deploy

GitHub Pages is enabled in repo Settings → Pages → "GitHub Actions" source. The workflow uploads the repo root as the artifact and publishes it. No build step.

To preview locally:

```bash
python3 -m http.server 8080
open http://127.0.0.1:8080
```

## Updating

- Marketing copy → edit `index.html`
- Privacy policy → keep in sync with [`sonder-clients/PRIVACY.md`](https://github.com/amayabdaniel/sonder-clients/blob/main/PRIVACY.md)
- Consent notice → keep in sync with [`sonder-clients/CONSENT.md`](https://github.com/amayabdaniel/sonder-clients/blob/main/CONSENT.md)
