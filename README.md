# Gymkhana Software — Marketing Site

The public marketing site for GymkhanaSoft, served at **gymkhanasoft.com** (and `www.gymkhanasoft.com`).

> This is the **marketing site only** — pricing, features, and a "get started" call to action. The actual application lives separately, behind a login, at `app.gymkhanasoft.com` (a different repo: `gymkhana-app`).

## What this is

A plain static site: one HTML page, a handful of images, a little vanilla JS. No build step, no framework, nothing to install or compile.

## Repository structure

```
gymkhana-site/
  index.html       — the whole page
  assets/          — images (hero, gallery photos, logo mark)
  README.md        — this file
  LICENSE          — proprietary, all rights reserved
```

## Running it locally

Just open `index.html` in a browser — it's a static page with no dependencies to install.

## Deployment

Deployed via **Cloudflare Pages**, connected to this GitHub repo — same workflow as the `gymkhana-app` repo:

- Framework preset: `None`
- Build command: *(none)*
- Build output directory: `/` (repo root, where `index.html` lives)
- Production branch: `main`
- Custom domains: **both** `gymkhanasoft.com` and `www.gymkhanasoft.com` are attached (this is the root domain — distinct from `app.gymkhanasoft.com`, which is the separate app repo/project)
- Any other branch gets an automatic preview URL; merge to `main` to go live

## Fonts & assets

- Fonts (Oswald, Source Sans 3) load from Google Fonts. Can be self-hosted later if we want zero external calls.
- Images are pre-optimized `.webp`, total well under 1 MB.

## Outstanding items

Search `index.html` for `TODO:` to find these inline, or track them here:

- [ ] Swap the placeholder circle logo for the real Canva logo (used in header, final CTA, and footer — `assets/horse-mark.png`)
- [ ] Point the "Download the app" buttons at the real downloadable app file once hosted
- [ ] Point "Get started" / "Get the cloud version" at the onboarding contact or `app.gymkhanasoft.com`
- [ ] Replace the "Annual — contact us" placeholder on the Premium price card with a real number
- [ ] Fill in the FAQ section (currently just a contact line)

## Related

- `gymkhana-app` — the actual application (Cloudflare Pages + Access + Worker/D1 backend), served at `app.gymkhanasoft.com`
