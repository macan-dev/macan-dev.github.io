# MACAN — Personal Site

Bilingual (فارسی / English) liquid-glass personal site for Macan.Dev — security researcher, reverse-engineer and developer.

Single self-contained `index.html` (no build step, no dependencies). Live GitHub projects + contributions load from the GitHub API in the browser.

## Publish on GitHub Pages → `macan-dev.github.io`

1. Sign in to GitHub as **macan-dev**.
2. Create a new repository named exactly **`macan-dev.github.io`** (Public).
3. Upload **all files** to the repo root — `index.html`, `.nojekyll`, `favicon.svg`, `favicon-32.png`, `favicon-16.png`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest` (drag them into the "uploading an existing file" area, then Commit).
4. Go to **Settings → Pages**. Under **Build and deployment**, set **Source = Deploy from a branch**, **Branch = `main` / `root`**, then **Save**.
5. Wait ~1 minute. Your site is live at **https://macan-dev.github.io**

That URL is permanent and free. Any time you edit `index.html` and commit, the site updates automatically.

### Notes
- `.nojekyll` tells GitHub Pages to serve the files as-is (skips Jekyll processing). Keep it in the repo root.
- The projects grid and contributions heatmap only populate when the page is served over http/https (GitHub Pages works). Opening the raw file locally shows the EasySNI / CFScanner fallback.

### Optional: a shorter / custom link
- **Custom domain:** buy a domain (e.g. `macan.dev`), add it under Settings → Pages → Custom domain, and point a CNAME to `macan-dev.github.io`.
- **Instant drag-drop alternative:** [tiiny.host](https://tiiny.host) — drop `index.html`, pick a name, get `yourname.tiiny.site` in seconds.
