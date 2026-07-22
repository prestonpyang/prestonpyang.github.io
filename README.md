# Preston Yang — Engineering Portfolio

Static site, no build step. Every page is a plain, self-contained HTML file (loads React/ReactDOM from a CDN at runtime) — open `index.html` directly in a browser or host the whole folder as-is.

## Pages
- `index.html` — About / home
- `Portfolio Projects.dc.html` — project listing (Mechanical Design, Manufacturing, Internships)
- `Contact.dc.html` — contact
- `Project - *.dc.html` — one page per project
- `RocketGuide.dc.html` — the flying rocket mascot (imported into every page)
- `support.js`, `image-slot.js` — runtime/component files, required as-is
- `assets/` — images used across the site

## Publish with GitHub Pages
1. Create a new GitHub repo and push this whole folder to it (root of the repo, or a `docs/` folder — either works).
2. In the repo: **Settings → Pages → Build and deployment → Deploy from a branch**, pick `main` and `/ (root)` (or `/docs`), save.
3. GitHub gives you a URL like `https://<username>.github.io/<repo>/` within a minute or two. `index.html` loads automatically at that root URL.

## Making updates
- **Small text/copy edits**: open any `.dc.html` file in a code editor and edit the visible text directly — it's plain HTML, safe to hand-edit.
- **Bigger changes (layout, new projects, styling, animations)**: bring this same folder back into this Claude design project (drag the whole folder back in, or just describe what you want changed) and continue from here — every file in this export is exactly what's live on the design canvas, so round-tripping is lossless.
- Don't rename `support.js` or `image-slot.js`, and don't remove the `<script src="./support.js">` tag at the top of each page — the pages won't render without it.
