# WorldWise Academy — Android-friendly PWA

A 12-week (84-lesson) politics and general-culture learning app built with plain HTML, CSS and JavaScript.

## Included
- 84 daily lesson entries, organised into 12 weeks
- Lesson notes, quiz questions, answer feedback and scores
- Dashboard, progress summary, study streak and weekly reflection
- Local progress saved in browser storage
- JSON export/import backup
- App manifest, 192px and 512px icons, service worker and offline app shell

## Deploy free with GitHub Pages
1. Sign in at https://github.com and create a public repository named `worldwise-academy`.
2. Upload the contents of this project folder, keeping `index.html` at the repository root.
3. In repository Settings → Pages, choose deploy from branch, select `main` and `/ (root)`, then Save.
4. Wait for the published URL. It will resemble `https://YOUR-USERNAME.github.io/worldwise-academy/`.
5. Open that HTTPS URL in Chrome on Android.

## Install on Android
1. Open your deployed HTTPS site in Chrome.
2. Tap Chrome's three-dot menu.
3. Choose **Install app** or **Add to Home screen** (wording varies).
4. Confirm. The icon should appear on your home screen.

## Test locally
PWA installation/service workers need HTTPS or localhost. In this folder run `python -m http.server 8000` and visit `http://localhost:8000` on the same device, or use a static server such as `npx serve .`.

## Data and privacy
- Progress is saved in local browser storage on this device; it does not sync across devices.
- Clearing site data may erase progress. Use Progress → Export backup regularly.
- Import a previously exported WorldWise JSON backup from Progress.
- Lessons are short foundations. Current news is linked externally and is not automatically fetched or bundled.
- This is a PWA, not a Play Store app.
## Updating
If you change files after deploying, increment the cache name in `sw.js` (e.g. `worldwise-academy-v2`) to ensure the updated shell is downloaded.
