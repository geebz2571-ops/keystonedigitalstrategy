# Keystone Digital Strategy — Website

Static, single-page marketing site. No build step, no dependencies (fonts load from
Google Fonts CDN). **This folder is the deploy root — deploy only this folder, never the
parent project folder (which contains confidential strategy documents).**

## Files
- `index.html` — the entire site (HTML + inline CSS + minimal JS)
- `og-image.png` — social-share preview image (1200×630)
- `favicon-64.png`, `apple-touch-icon.png` — icons
- `vercel.json` — security headers + asset caching
- `robots.txt`, `sitemap.xml` — SEO

## Edit
Everything visible is in `index.html`. To swap the recreated logo for a raster file,
drop `logo.png` into this folder and follow the `LOGO PLACEHOLDER` comment in the hero.

## Deploy (Vercel)
**CLI:** from this folder, `vercel` then `vercel --prod`.
**Git:** push this folder to a repo and import it at vercel.com.

## Domain & email
Domain registered at Squarespace. Web records point to Vercel; email (MX) points to
Google Workspace. Keep the two sets of DNS records separate so both work at once.
