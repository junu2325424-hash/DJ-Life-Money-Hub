# DJ's LIFE & MONEY HUB — Free starter PWA

## Included
- Mobile-first finance tracker with income, expenses, account balances, brand receivables, lending/borrowing, product return deadlines, savings goals.
- Local/offline storage in the browser.
- JSON backup restore and CSV transaction export.
- Installable PWA shell and app icon.

## Important limitations
This starter stores personal records only in the current browser on the current device. Cloud login/sync is NOT enabled yet. Do not upload personal records or backup files to a public GitHub repository. Export a JSON backup regularly and keep it in a private location.

Browser notifications require permission. The app checks deadlines when it is opened and may display notifications then. This is not a guaranteed scheduled alarm if the browser is fully closed or Android restricts background activity.

## Publish on GitHub Pages
1. Create a private/public repository for source (source code contains no personal finance records).
2. Upload `index.html`, `manifest.json`, `icon.svg`, and `sw.js` to repository root.
3. Settings → Pages → Deploy from branch → `main` → `/ (root)` → Save.
4. Open the Pages URL in Chrome → menu → Add to Home screen / Install app.

## Cloud sync next
For private cloud sync, create a Firebase project on the free Spark plan, enable Authentication and Firestore, then add a per-user Firestore data model and strict security rules before connecting it. The current code deliberately does not claim cloud backup. Firebase usage limits and product terms can change; check the current Firebase console before deployment.
