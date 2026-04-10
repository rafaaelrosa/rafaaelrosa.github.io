# rafaaelrosa.github.io

GitHub **user** Pages site. Hosts only [`app-ads.txt`](./app-ads.txt) at the site root so [Google AdMob](https://support.google.com/admob/answer/9363762) can fetch:

`https://rafaaelrosa.github.io/app-ads.txt`

The Deus.iA support page stays in the separate [`deus-ai-support`](https://github.com/rafaaelrosa/deus-ai-support) repository.

## Publish

1. Create a **public** GitHub repository named exactly **`rafaaelrosa.github.io`** (must match your username).
2. Add this folder as the repo root (or push from below).
3. **Settings → Pages:** deploy from branch **`main`**, folder **`/ (root)`**.
4. Verify in a browser: `https://rafaaelrosa.github.io/app-ads.txt` shows one line of plain text.
5. In AdMob: **Check for updates** on app-ads.txt (verification can take hours).

## Git remote (after you create the empty repo on GitHub)

```bash
cd /path/to/rafaaelrosa.github.io
git remote add origin https://github.com/rafaaelrosa/rafaaelrosa.github.io.git
git push -u origin main
```

Replace the URL with the one GitHub shows if different.
