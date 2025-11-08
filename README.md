# Inovasi Group Website

Static single-page website for Inovasi Group showcasing AI Technology and Finance solutions with a small portfolio: Dinamika Prima Servitama, Klikcash.id, and AtlasBox (Q2/26). The site is intentionally lightweight (pure HTML/CSS, no build tools) so it can be opened directly from disk or hosted on any static host.

## Tech Stack
- **HTML**: `index.html`
- **CSS**: `assets/css/style.css`
- **Assets**: `assets/img/`

## Project Structure
```
inovasi-group-website/
├─ index.html                # Page markup
├─ assets/
│  ├─ css/
│  │  └─ style.css          # All styles (light theme)
│  └─ img/                  # Images and logos
│     ├─ inovasi-logo.png   # Header logo
│     ├─ uiphone.png        # Klikcash illustration
│     ├─ dps.png            # Dinamika Prima Servitama logo
│     ├─ about-5.webp       # Content image
│     ├─ finance.jpg        # Content image
│     ├─ atlasbox.jpg       # AtlasBox product image (fallback to atlasbox.png)
│     ├─ atlasbox.png       # Alternate AtlasBox image
│     └─ ojk.png            # OJK logo used in portfolio cards 1–2
└─ README.md
```

## Running Locally
- Open `index.html` directly in your browser, or
- Serve the folder with any static server (recommended for correct caching):

```bash
# Python 3
python3 -m http.server 8080
# then open http://localhost:8080
```

## Editing Content
- **Header logo**: Update `assets/img/inovasi-logo.png`.
- **Hero text/CTA**: See the `<header>` block in `index.html`.
- **Sections**: Edit copy directly in `index.html`.
- **Portfolio**: Update cards inside the `#portfolio` section.
  - Logos/images live in `assets/img/`.
  - AtlasBox card uses `assets/img/atlasbox.jpg` with a fallback to `assets/img/atlasbox.png`.
  - OJK logo under the first two cards uses `assets/img/ojk.png`.

## Styling
- Primary stylesheet: `assets/css/style.css`.
- Notable rules:
  - `.logo`: centers the header logo.
  - `.portfolio` and `.card`: responsive grid with equal-height cards.
  - `.ojk`: small OJK badge aligned at the card bottom for tidy alignment.

## Assets & Notes
- Prefer PNG or SVG for logos. Use transparent backgrounds when needed.
- All external images have been cached locally to ensure offline availability.

## Deployment
- Any static host works (Netlify, GitHub Pages, Vercel, S3, etc.).
- Upload the folder as-is or point the host to its root.

## License
Content and assets belong to their respective owners. Internal code is provided as-is for Inovasi Group use.
