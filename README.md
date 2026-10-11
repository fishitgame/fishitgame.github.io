# Fish It! - Links

Link-in-bio page for **Fish It! Sort the Aquarium Shop**: https://fishitgame.github.io/

Static page, no build step, no tracking, **no JavaScript**, no third-party requests
(fonts are self-hosted). Served by GitHub Pages from `main`.

## Security
- Strict Content-Security-Policy (meta tag): `default-src 'none'`, only this site's own
  fonts/images and the one inline `<style>` block (allowed by its SHA-256 hash).
- **If you edit anything inside `<style>`, the hash in the CSP meta tag must be updated**,
  otherwise the page loses all styling. Recompute:
  `python -c "import re,hashlib,base64;t=open('index.html',encoding='utf-8').read();s=t.split('<style>',1)[1].split('</style>',1)[0];print(base64.b64encode(hashlib.sha256(s.encode()).digest()).decode())"`
- `.gitattributes` keeps line endings byte-exact (the hash depends on them).

- `index.html` - the page (logo embedded)
- `og-image.png` - share preview (Discord / Instagram / WhatsApp)
- `favicon.png`
- `fonts/` - Fredoka & Nunito (SIL Open Font License, see `fonts/OFL-*.txt`), Latin subset

When the Steam store page goes live, replace the `<div class="soon">` Steam block in
`index.html` with a link card (see the comment above it) and push.
