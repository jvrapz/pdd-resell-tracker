PDD Reseller Tracker — PWA package

Files:
- index.html: your inventory tracker
- manifest.webmanifest: installable app information
- service-worker.js: offline app shell cache
- icon-192.png and icon-512.png: home-screen icons

FREE DEPLOYMENT (GitHub Pages):
1. Create/sign in to a GitHub account.
2. Create a new public repository named pdd-reseller-tracker.
3. Upload all five files from this folder to the repository root (not the folder itself).
4. In the repository, open Settings > Pages.
5. Under Build and deployment, choose Deploy from a branch.
6. Choose branch main and folder /(root), then Save.
7. Wait for GitHub Pages to publish. Your site URL will look like:
   https://YOUR-USERNAME.github.io/pdd-reseller-tracker/
8. Open the URL in Chrome on Android or Edge/Chrome on Windows.
9. Android: Chrome menu ⋮ > Install app (or Add to Home screen).
   Windows: browser install icon in the address bar, or menu > Install PDD Reseller Tracker.
10. Open the installed app from the home screen/Start menu.

Important:
- Use the published HTTPS URL; opening index.html directly from Downloads will not enable PWA installation.
- This package caches the app shell for offline opening. It does NOT synchronize data between devices.
- The current tracker saves data in browser storage on each device. Export a JSON backup regularly.
- If you update the app later, increment CACHE_NAME in service-worker.js (e.g. pdd-tracker-v2) so browsers fetch the new version.
