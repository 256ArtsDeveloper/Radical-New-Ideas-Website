# Radical New Ideas Website

Static site, no build step. Preview: `python3 -m http.server 8123` from the repo root.

- `index.html` — homepage. Add one `<a class="article">` card per article in `#articles`, newest first.
- `articles/<slug>/index.html` — each article is a single page with inline CSS/JS/SVG. Photos live in `articles/<slug>/images/` as JXL only (no fallbacks), ≤1600px; lossless-transcode JPEG sources with `cjxl --lossless_jpeg=1`. Full-res originals go in iCloud `Repo Assets/Radical New Ideas Website/Photo Originals/`.
- Colors are CSS tokens on `:root` with dark-mode overrides; keep both in sync when adding tokens.

## Writing style

- Lead with the pain, not the manifesto. Readers latch onto solutions, so open on a painful, recurring bottleneck people already feel (and Google) — waiting in lines, fighting bureaucracy — then present the radical idea as the fix.
- Ground claims in concrete numbers, sources and everyday examples. Titles and deks are plain and provocative; headings are short claims.
- Short sentences, no jargon. Cut anything that doesn't move the argument.

## Presentation style

- Scrollytelling: each section is a scroll-driven scene with heavy graphics — animated SVG diagrams, charts, photos, reveals tied to scroll.
- It must still read like an article: continuous prose carries the argument; visuals illustrate it, never replace it. Works top-to-bottom without interacting.
- Need a photo or image asset? Ask Jayden rather than using stock or generating one.
