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

## Known Issue — Ignicell Button Still Showing on Live Site
**Status:** Unresolved as of Apr 14 2026

The live site (nutravybe.com) still shows a yellow "Ignicell Comprar" button in the navigation bar even after pushing clean files to GitHub.

**Root cause:** The Hostinger git auto-deploy does NOT appear to be running. The HTML files on Hostinger were likely uploaded manually before the git integration was set up, and git pushes are not overwriting them.

**Fix needed:**
1. Go to Hostinger hPanel → Git
2. Verify the auto-deploy webhook is active for the `main` branch
3. Manually trigger a redeployment if available
4. OR use Hostinger File Manager to manually delete/replace the old HTML files with the clean git versions

## Content Notes
- All articles are in Brazilian Portuguese
- Author: Amanda Biavati, Nutricionista CRN 22509
- Images are embedded as base64 (no external image dependencies)
- Article content is in `<p>` tags inside `.article-content > .article-container`
- Canonical URLs point to `https://nutravybe.com/`

## What Still Needs To Be Done
- [ ] Confirm Hostinger git auto-deploy is working (verify live site after next push)
- [ ] Resolve Ignicell button on live site (see Known Issue above)
- [ ] Add any additional articles if needed
