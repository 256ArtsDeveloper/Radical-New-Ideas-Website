# Radical New Ideas Website

Static site, no build step. Preview: `python3 -m http.server 8123` from the repo root.

- `index.html` — homepage. Add one `<a class="article">` card per article in `#articles`, newest first.
- `articles/<slug>/index.html` — each article is a single self-contained page (inline CSS/JS/SVG, no external assets). `outline.md` and `draft.md` beside it are research/copy, not served content.
- Colors are CSS tokens on `:root` with dark-mode overrides; keep both in sync when adding tokens.
