# HomeFinder India — Free starter prototype

## What's included
- Responsive property search UI for rent and buy
- Search by city/state/locality, type, budget, bedrooms, owner/agent
- Add a listing form
- Save favourites
- Property detail view and WhatsApp contact link for user-created listings
- PWA manifest and basic service worker

## Important limitations
This is a front-end prototype. Listings and saved favourites are stored in the browser's localStorage on one device. They are NOT shared with other users and there is no login, server database, secure image upload, moderation, or verified-owner process yet. The included sample listings are illustrative and do not have real contact details.

## Run on your computer
1. Install a current Node.js LTS version if you do not already have one (optional for the static website).
2. Open this folder in VS Code.
3. To preview quickly, open `index.html` in a browser. Some PWA features require HTTPS or localhost.
4. For a local server, from this folder run: `npx serve .` and open the local URL it prints.

## Free website deployment
1. Create a GitHub account and a new **public** repository named `homefinder-india`.
2. Upload `index.html`, `manifest.json`, and `service-worker.js`.
3. In repository Settings → Pages, select deployment from the main branch/root folder and save.
4. GitHub will show the published `https://YOUR-USERNAME.github.io/homefinder-india/` URL.
5. HTTPS hosting allows users to add the site to their phone home screen. Recheck the site after each change.

## Android path
- Easiest no-cost test: open the deployed site in Chrome on Android → menu → **Add to Home screen** (the exact wording can vary). This creates an app-like shortcut, not a Play Store release.
- For a real native Android wrapper later, use Expo/React Native or a PWA-to-APK workflow and test on a device. Google Play publishing generally requires a one-time US$25 developer registration fee; APK sharing can avoid the store fee but users must install it themselves.
- This HTML version is not a native Android APK yet. It is a responsive web/PWA starting point.

## Next production steps
1. Create Firebase project on the Spark plan and configure email authentication.
2. Move listings into Firestore with access rules so only signed-in owners/agents can create/edit their own listings.
3. Add approved image storage, listing reporting, moderation, spam controls, and delete/edit workflows.
4. Verify phone numbers and build owner/agent verification checks.
5. Add privacy policy, terms, abuse contact, data deletion, and appropriate property/legal disclosures before public launch.
6. Test Firebase quotas and billing settings carefully; do not attach a billing account unless you understand the possible charges.

## Monetisation later
Potential options include clearly marked ads, paid featured listings, and optional agent tools. Keep basic search accessible. Revenue is not guaranteed.
