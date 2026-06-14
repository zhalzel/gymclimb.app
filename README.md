# gymclimb.app

Marketing and support site for **Gym Climb**, a lightweight indoor climbing
logbook for iPhone and Apple Watch.

## This repo is the source of truth for the website

The live site at <https://gymclimb.app> is served by **GitHub Pages from this
repo** (`main` branch, root path). The app source lives separately in
[`zhalzel/Climbing`](https://github.com/zhalzel/Climbing) — do **not** edit the
site from there. Any `docs/` folder in the app repo is not deployed.

## Structure

```
index.html          Landing page
privacy/index.html  Privacy policy
support/index.html  Support page
assets/             CSS, app icon, screenshots, social preview (og-image.png)
sitemap.xml         Search-engine sitemap
robots.txt          Crawl rules
site.webmanifest    Web app manifest
CNAME               Custom domain (gymclimb.app)
.nojekyll           Serve files as-is (skip Jekyll processing)
```

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages rebuilds automatically within a minute or two.

## Updating the App Store link

Until the app ships, the hero shows a "coming soon" badge. When the App Store
listing is live, search `index.html` for `APP STORE LINK` and follow the inline
comment to swap the placeholder for the real download badge and URL.
