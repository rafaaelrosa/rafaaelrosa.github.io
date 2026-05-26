# rafaaelrosa.github.io

GitHub **user** Pages site for [Rafael Rosa](https://github.com/rafaaelrosa). Hosts the developer landing page and the public-facing legal / support pages for **Deus.iA**, plus [`app-ads.txt`](./app-ads.txt) at the site root so [Google AdMob](https://support.google.com/admob/answer/9363762) can fetch it.

## Live URLs

| File | URL | Used by |
|---|---|---|
| `app-ads.txt` | `https://rafaaelrosa.github.io/app-ads.txt` | AdMob authorization (hostname-only fetch) |
| `index.html` | `https://rafaaelrosa.github.io/` | App Store Connect → **Marketing URL** |
| `privacy.html` | `https://rafaaelrosa.github.io/privacy.html` | App Store Connect → **App Privacy → Privacy Policy URL**; Play Console → Privacy policy |
| `support.html` | `https://rafaaelrosa.github.io/support.html` | App Store Connect → **Support URL** |
| `terms.html` | `https://rafaaelrosa.github.io/terms.html` | In-app + App Description "Terms of Use" link |

## Publish

1. Create a **public** GitHub repository named exactly **`rafaaelrosa.github.io`** (must match your username).
2. **Settings → Pages:** deploy from branch **`main`**, folder **`/ (root)`**.
3. Verify in a browser: each URL above returns HTTP 200 and renders.
4. In AdMob: **Apps → Deus.iA → app-ads.txt → Check for updates** (verification can take up to 24h).

## Edit

- Pure static HTML + inline CSS. No build step.
- Push to `main` → GitHub Pages republishes within ~60s.
- After publishing a new URL in App Store Connect (Privacy / Support / Marketing), confirm the link opens with no auth wall.

## Notes

- The `app-ads.txt` content (publisher ID + `DIRECT` + certification ID) must match exactly what AdMob shows — do not paraphrase.
- AdMob crawler always hits `https://<hostname>/app-ads.txt`. Adding extra files to this repo does **not** affect detection.
- Privacy / Terms are mirrored from the canonical sources; if either changes, update the HTML here and bump the "Last updated" date.
