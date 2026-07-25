# Thalify website

Static site, no build step. Branded to the app icon (amber→green progress gauge on dark green).

## Files
index.html · privacy.html · support.html · CNAME
icon-192.png · icon-512.png · favicon-32.png · apple-touch-icon.png  (all referenced — keep them)

## Signature
The hero is a semicircular gauge that sweeps amber→green (matching the icon) as the AI
parses a meal and the calorie readout climbs. Section dividers echo the same arc. The icon
is the nav mark, footer mark, favicon, and og:image.

## Deploy (GitHub Pages)
Upload ALL files (including the 4 PNGs) to repo root. Settings → Pages → deploy from main /(root).
Cloudflare DNS: four A records @ → 185.199.108–111.153, CNAME www → eharinathkumar.github.io, all DNS-only (grey).
Settings → Pages → Custom domain thalify.app → Enforce HTTPS.

## Swap before launch
- Play Store URL: two "Get it on Android" links + #playLink.
- Demo video: replace the .vplace block in .videobox.
- Screenshots: replace the three .ph divs with <img> tags.

## Palette (from icon)
ink #191F13 · cream #F1EDE2 · green #4C9A45 · amber #F5A623
Space Grotesk (display) / Inter (body) / IBM Plex Mono (data)
