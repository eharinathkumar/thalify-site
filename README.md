# Thalify website

Static marketing site for Thalify. No build step — plain HTML/CSS/JS.

## Files
- `index.html` — landing page (interactive thali hero)
- `privacy.html` — privacy policy (required by Google Play / Apple)
- `support.html` — support page (required if you ship on iOS)
- `CNAME` — custom domain for GitHub Pages

## Deploy
1. Create a repo (e.g. `thalify-site`), upload these files.
2. Settings → Pages → Deploy from branch `main`, folder `/ (root)`.
3. Settings → Pages → Custom domain → `thalify.app` → Save. Tick **Enforce HTTPS**.
4. At your registrar, add DNS records:
   - A records for the apex (`thalify.app`) → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - CNAME `www` → `eharinathkumar.github.io`

## Before going live — swap in real assets
- **Play Store link**: in `index.html`, set `href` on the two "Get it on Android" buttons and `#playLink`.
  Official Google Play badge assets: https://play.google.com/intl/en_us/badges/
  (Use Google's badge image rather than a text button once you have the store URL.)
- **Demo video**: replace the `.vplaceholder` block inside `.videobox` with either
  `<video src="demo.mp4" poster="demo-poster.jpg" autoplay muted loop playsinline></video>`
  or a YouTube `<iframe>`. Keep local files under ~5 MB.
- **Screenshots**: replace the three `.ph` placeholder divs with
  `<img src="screenshot-today.png" alt="Today tab showing calorie and protein rings">` etc.
- **Contact email**: currently `thalifit.admin@gmail.com` in the footer, privacy and support pages.

## Notes
- The thali hero pulls its dishes from the `DISHES` array at the bottom of `index.html` — edit freely.
- Fonts load from Google Fonts. To go fully self-hosted later, download Fraunces / Public Sans / IBM Plex Mono into `/fonts`.
- Colours are CSS variables in `:root`, matching the app's palette.
