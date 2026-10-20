# Nua Harvest website

Static site (no build step). Files:

- `index.html` – the store (cart, delivery form, WhatsApp ordering)
- `nua_harvest_hero.mp4` – hero video (keep this exact name, `index.html` loads it)
- `poster.jpg` – image shown while the video loads
- `.nojekyll` – tells GitHub Pages to serve the files as they are

## Publish on GitHub Pages
1. Create a public repository (e.g. `nua-harvest`).
2. Upload **all files in this folder** (drag and drop works, including `.nojekyll`).
3. Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.
4. Live in about a minute at `https://<username>.github.io/<repo>/`.

## Custom domain
Settings → Pages → Custom domain, enter your domain, then add the DNS records GitHub shows at your registrar. Enable "Enforce HTTPS" once available.

## Edit store settings
Search `CFG` near the top of the script in `index.html`:
`whatsapp` (number with country code, no +), `payLink` (optional Razorpay link, hidden while empty), `freeShip` (free-shipping threshold).
Prices and sizes are in the `PRODUCTS` list just below.
