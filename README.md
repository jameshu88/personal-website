# itsjameshuang.live

Personal site for James Huang. Single-page, dark, editorial. Built as the founder-facing surface for Seraphim Labs / FormLab AI.

## Stack
Plain HTML, CSS, and a small vanilla-JS reveal/nav script. No build step, no framework, no dependencies. Fonts served from Google Fonts (Fraunces, Inter, JetBrains Mono).

## Files
- `index.html` — the entire site
- `style.css` — design system and layout
- `script.js` — sticky-nav behavior + IntersectionObserver reveals
- `CNAME` — custom domain (`itsjameshuang.live`)

## Local preview
Any static server works:

```
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy (GitHub Pages)
1. Commit and push to `main` (or whichever branch Pages is configured to serve).
2. In the repo settings → Pages, set source to the `main` branch, root (`/`).
3. The `CNAME` file pins the custom domain. Ensure DNS for `itsjameshuang.live` points to GitHub Pages (`A` records to the GitHub Pages IPs, or a `CNAME` record to `jameshu88.github.io`).
4. Allow a few minutes for the cert to provision; enable "Enforce HTTPS".
