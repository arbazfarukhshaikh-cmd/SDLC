# QA Tester Academy — iPhone Home Screen app

This is an installable Progressive Web App (PWA). It is not an App Store binary or a native Xcode project.

## Files
- `index.html` — complete app (lessons, bug lab, quiz, SQL practice, API concepts, automation examples, interview prep, notes and progress).
- `manifest.webmanifest` — install metadata.
- `service-worker.js` — offline app-shell caching.
- `icon-192.png`, `icon-512.png` — app icons.

## Publish it (required for iPhone installation)
PWAs need to be served over HTTPS (or localhost). Easiest options:
1. Create a free GitHub account and a new public repository named `qa-tester-academy`.
2. Upload all files from this folder to the repository root.
3. In repository Settings → Pages, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
4. Wait for GitHub Pages to publish the HTTPS website. The URL will look like `https://YOUR-USERNAME.github.io/qa-tester-academy/`.

Alternative: deploy the folder using Netlify or another HTTPS static hosting provider.

## Add to iPhone
1. Open the published HTTPS URL in Safari on your iPhone.
2. Tap Share (square with upward arrow).
3. Scroll and choose **Add to Home Screen**.
4. Keep **Open as Web App** enabled if shown, then tap Add.
5. Launch **QA Academy** from the new Home Screen icon.

## Notes
- Lessons completed, best quiz score, bug reports and notes are saved in browser local storage on that device.
- Use “Export my progress (JSON)” to back up your progress.
- Clearing Safari website data can erase locally saved progress.
- The service worker caches the app shell for offline reopening after the first successful online visit. External links and any future online services still need internet.
- This starter app does not connect to a backend, provide user accounts, issue accredited certificates, or run real browser/device automation. SQL exercises are guided query checks, not a live database.
- If you later want App Store distribution, this PWA can be wrapped or rebuilt as a native iOS app, which requires Apple developer tooling and signing.
