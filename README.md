# Fish It! - Links

Link-in-bio page for **Fish It! Sort the Aquarium Shop**: https://fishitgame.github.io/

Static page, no build step, no tracking, **no JavaScript**, no third-party requests
(fonts are self-hosted). Served by GitHub Pages from `main`.

## Security
- Strict Content-Security-Policy (meta tag): `default-src 'none'`; styles, fonts and images
  only from this site itself (`'self'`, plus the embedded logo as a `data:` image).
  No scripts can run at all.
- All styling lives in `style.css` - edit it freely, no hashes to update.

## Files
- `index.html` - the page (logo embedded)
- `style.css` - all styling
- `og-image.png` - share preview (Discord / Instagram / WhatsApp)
- `favicon.png`
- `fonts/` - Fredoka & Nunito (SIL Open Font License, see `fonts/OFL-*.txt`), Latin subset

When the Steam store page goes live, replace the `<div class="soon">` Steam block in
`index.html` with a link card (see the comment above it) and push.
