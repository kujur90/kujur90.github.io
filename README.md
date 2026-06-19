# Portfolio

Static site — no build step. Just HTML, CSS, and JS.

## Before you deploy — fill these in

- `index.html`
  - `<span class="muted">[Last Name]</span>` → your surname
  - `mailto:your.email@example.com` → your real email (appears twice: nav-less, contact section)
  - `<title>` and the `og:` meta tags if you want a custom name in tab/share previews
  - sesta.in URL in the MIS record currently has no link (no public URL on file) — add one if it's public
  - Experience dates ("present" / no dates) — add start year if you want them

## Deploy to GitHub Pages

**Option A — user site (`https://kujur90.github.io`)**

```bash
# create a repo on GitHub named exactly: kujur90.github.io
cd portfolio
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/kujur90/kujur90.github.io.git
git push -u origin main
```

Pages will auto-publish at `https://kujur90.github.io` within a minute or two — no settings change needed for this repo name.

**Option B — project site (any repo name)**

```bash
cd portfolio
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/kujur90/portfolio.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Source → Deploy from branch → `main` / `(root)`**.
Site will be live at `https://kujur90.github.io/portfolio/`.

## Structure

```
index.html
css/style.css
js/main.js
```
