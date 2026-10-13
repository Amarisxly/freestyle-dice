# Freestyle Dice (PWA)

Roll a word, talk for a guided minute. Works offline once installed.

## Files
- `index.html` – the whole app (1,015 words, eight design styles)
- `manifest.webmanifest` – name, icons, colors for installing
- `sw.js` – service worker for offline use
- `icons/` – app icons (192, 512, maskable, Apple touch, favicon)

## Put it online (pick one, all free)
A PWA must be served over **https**. Opening `index.html` straight from your computer works, but it won't install or go offline.

**Netlify Drop (easiest):** go to https://app.netlify.com/drop and drag this whole folder onto the page. You get a link in seconds.

**GitHub Pages:** create a repository, upload these files to it, then Settings → Pages → Deploy from branch → `main` / root.

**Vercel:** `npx vercel` inside this folder.

## Install on your phone
- **iPhone (Safari):** open the link → Share → **Add to Home Screen**.
- **Android (Chrome):** open the link → menu → **Install app**.
- **Desktop Chrome / Edge:** click the install icon in the address bar.

## Updating
After you change `index.html`, bump `VERSION` in `sw.js` (for example `fd-v2`) so installed copies pick up the new version.
