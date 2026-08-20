# Dugout Baseball — GitHub Pages Ready

This folder is ready to upload directly to a GitHub repository.

## Files

- `index.html` — the Dugout app
- `manifest.json` — makes the site installable as a web app/PWA
- `service-worker.js` — caches the basic app shell for offline startup
- `icon-192.png` and `icon-512.png` — app/Home Screen icons
- `.nojekyll` — tells GitHub Pages to serve the files exactly as uploaded

## Put it on GitHub

1. Sign in to GitHub.
2. Create a new repository, for example `dugout-baseball`.
3. Open the repository and choose **Add file → Upload files**.
4. Upload **all files from this folder** into the root of the repository. Do not upload the outer folder itself as a nested folder.
5. Click **Commit changes**.
6. Open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Choose branch **main** and folder **/(root)**, then click **Save**.
9. Wait a minute or two. GitHub will show the public Pages URL.

## Install on iPad

1. Open the GitHub Pages URL in Safari.
2. Tap the Share button.
3. Choose **Add to Home Screen**.
4. Open Dugout from the new Home Screen icon.
5. Landscape orientation is recommended.

## Updating the app later

Replace `index.html` with your newer version and commit it to GitHub. If you make major PWA changes, also increase the cache version near the top of `service-worker.js` from `dugout-shell-v1` to something like `dugout-shell-v2`.

## Important prototype limitation

Uploaded videos/games are still browser-session/local data in the current prototype. GitHub Pages hosts the app itself; it does not provide permanent database or cloud video storage.
