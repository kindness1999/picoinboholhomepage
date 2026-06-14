# picoinbohol.com

PICO HOUSE & PICO DIVE static website.

## GitHub Pages

1. Repository **Settings → Pages**
2. **Source:** Deploy from branch `main`, folder `/ (root)`
3. **Custom domain:** `www.picoinbohol.com` (CNAME file included)
4. At your domain registrar (HostingKR DNS), point to GitHub Pages:
   - `www` → CNAME → `kindness1999.github.io` (or GitHub Pages target shown in Settings)
   - Apex `picoinbohol.com` → A records to GitHub Pages IPs (optional redirect to www)

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
