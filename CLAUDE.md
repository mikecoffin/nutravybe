# NutraVybe — Creatina Content Site

## Project Overview
Static HTML content site about creatina (creatine), hosted on Hostinger at **nutravybe.com**.
49 HTML articles + index, all self-contained with embedded images (base64).

## Tech Stack
- **Type:** Pure static HTML (no build step, no framework)
- **Hosting:** Hostinger (nutravybe.com)
- **Git repo:** https://github.com/mikecoffin/nutravybe
- **Deploy:** Hostinger auto-deploys on push to `main` branch via GitHub integration
- **Local path:** `C:\Users\ateda\OneDrive\Área de Trabalho\nutravybe\creatina-content\creatina-html-site`

## File Structure
```
creatina-html-site/
├── index.html                  # Homepage — article grid
├── *.html                      # 49 article pages
├── sitemap.xml
├── robots.txt
└── CLAUDE.md
```

## Navigation (all pages)
Every HTML file shares the same `<header>` nav:
```
Início | Guia Completo | Como Tomar | Tipos | FAQ
```
No external CTA buttons, no affiliate links in the nav.

## What Has Been Done
- [x] 49 article HTML files created (creatina topical authority site)
- [x] index.html with article grid
- [x] sitemap.xml and robots.txt
- [x] Git repo created and pushed to GitHub (mikecoffin/nutravybe)
- [x] Hostinger connected to GitHub for auto-deploy
- [x] Removed "Ignicell Comprar" CTA button from all pages (nav cleaned)
- [x] All 49 HTML files committed and pushed to force Hostinger redeploy (Apr 2026)

## Hostinger Deployment Setup
- **Primary domain on account:** segredodaproteinavegetal.com.br (Hostinger shows this in logs even for nutravybe.com)
- **nutravybe.com document root:** `public_html/` (same root as primary domain — no subfolder)
- **Git install path:** `public_html` (correct — deploys directly to nutravybe.com's root)
- **Auto Deployment:** Must be toggled ON in hPanel → Git for pushes to auto-deploy
- Build log shows "on segredodaproteinavegetal.com.br" — this is normal, it's just the account's primary domain label

## Content Notes
- All articles are in Brazilian Portuguese
- Author: Amanda Biavati, Nutricionista CRN 22509
- Images are embedded as base64 (no external image dependencies)
- Article content is in `<p>` tags inside `.article-content > .article-container`
- Canonical URLs point to `https://nutravybe.com/`

## What Still Needs To Be Done
- [ ] Enable Auto Deployment in hPanel → Git (toggle ON)
- [ ] Confirm Ignicell button is gone after hard refresh / incognito (likely browser cache)
- [ ] Add any additional articles if needed
