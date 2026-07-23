# picoinbohol.com

PICO HOUSE & PICO DIVE static website.

## GitHub Pages

This site is published with the **GitHub Actions** workflow in `.github/workflows/deploy-pages.yml`.

1. Repository **Settings → Pages**
2. **Source:** GitHub Actions
3. **Custom domain:** `www.picoinbohol.com` (CNAME file included)
4. At your domain registrar (HostingKR DNS), point to GitHub Pages:
   - `www` → CNAME → `kindness1999.github.io` (or GitHub Pages target shown in Settings)
   - Apex `picoinbohol.com` → A records to GitHub Pages IPs (optional redirect to www)

### If you see `There isn't a GitHub Pages site here.`

That message means GitHub Pages is **unpublished / disabled** for this repository (`has_pages: false`), not that the HTML is broken.

Recover with:

1. Open [Settings → Pages](https://github.com/kindness1999/picoinboholhomepage/settings/pages)
2. Set **Source** to **GitHub Actions**
3. Ensure the custom domain is `www.picoinbohol.com`
4. Merge the latest deploy fix into `main` (or run **Actions → Deploy to GitHub Pages → Run workflow**)
5. Wait for the workflow to finish, then hard-refresh the site

Notes:

- This repository is currently **private**. On GitHub Free, making a repo private can automatically unpublish Pages.
- If Pages cannot be enabled while private, either make the repository **public**, or use a paid GitHub plan that supports Pages on private repositories.
- DNS can look correct while Pages is off; you will still get the GitHub Pages 404 page.

## Structure

```
index.html          Home
pico_house_*.html   Pico House (en/kr)
pico_dive_*.html    Pico Dive (en/kr)
open.html           Open notice
taeho_*.html        Taeho pages
css/                Styles
js/                 Scripts
image/              Photos
logo/               Logos & icons
```
