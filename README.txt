LINGUALAB MOBILE (PWA)

This package turns LinguaLab into an installable Progressive Web App (PWA).
It is not an APK. It can be installed from a secure HTTPS website and can cache the core app for offline use after the first visit.

IMPORTANT ABOUT INSTALLATION
- A service worker and install prompt generally require HTTPS (or localhost). Opening index.html directly from the file manager is not enough for PWA installation/offline caching.
- Publish the contents of this folder to a static HTTPS host such as GitHub Pages or Netlify. Then open that HTTPS URL in Chrome on Android.
- In Chrome, use the three-dot menu and choose “Install app” or “Add to Home screen” (wording may vary).
- On iPhone, open the HTTPS site in Safari, tap Share, then “Add to Home Screen”.

DATA
- Existing app progress uses browser storage, which is usually tied to the same site origin and browser profile. Switching from a local HTML file to the hosted PWA may not carry over old progress automatically.
- Keep browser/site data intact and use any available export/backup feature before switching devices or browsers.
- Offline caching makes the app shell available; browser speech recognition and speech synthesis may still need browser support and/or an internet connection.

CONTENTS
- index.html: LinguaLab app
- manifest.webmanifest: installation metadata
- sw.js: offline cache service worker
- icons/: app icons
