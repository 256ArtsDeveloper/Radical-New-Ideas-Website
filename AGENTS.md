# Radical New Ideas Website

Static site, no build step. Preview: `python3 -m http.server 8123` from the repo root.

- `index.html` — homepage. Add one `<a class="article">` card per article in `#articles`, newest first.
- `articles/<slug>/index.html` — each article is a single page with inline CSS/JS/SVG. Photos live in `articles/<slug>/images/` as JXL only (no fallbacks), ≤1600px; lossless-transcode JPEG sources with `cjxl --lossless_jpeg=1`. Full-res originals go in iCloud `Repo Assets/Radical New Ideas Website/Photo Originals/`.
- Colors are CSS tokens on `:root` with dark-mode overrides; keep both in sync when adding tokens.
