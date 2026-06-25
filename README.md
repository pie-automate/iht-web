# iht-web

Marketing landing page for **Indie Hacker Tycoon** — a satirical solo-founder career sim for iOS.

Single static page, no build step. Open `index.html` locally, or serve the folder
(`python3 -m http.server`). Reuses the game's design system (OKLCH tokens,
Space Grotesk + JetBrains Mono).

## Deploy (GitHub Pages)
Settings → Pages → **Source: Deploy from a branch → `main` / `/ (root)`**.
Lives at `https://pie-automate.github.io/iht-web/`. Put Cloudflare in front for a
custom domain + CDN/SSL (add a `CNAME` file with the domain).

## Going live — TODO
- **TestFlight link:** set `TESTFLIGHT_URL` in `index.html` to the public TestFlight
  link; until then the CTAs show "opening soon". 
- **og tags:** make `og:image` / `twitter:image` absolute (`https://<domain>/og.png`)
  and add `og:url` once the domain is set.

`og.png` (1200×630 share card) is generated from the app icon + brand.
