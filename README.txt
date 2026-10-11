MAFIA — PASS & PLAY (INSTALLABLE WEB APP)

WHAT'S INCLUDED
- index.html: the game
- manifest.webmanifest: install name, icon and display settings
- service-worker.js: caches the app for offline use after the first visit
- icons/: app icons for Android and other platforms

IMPORTANT
To install it like an app, the files must be served from an HTTPS website (or localhost). Opening index.html directly from Downloads will still run the game, but browser installation and offline caching won't activate from file:// URLs.

EASY FREE HOSTING OPTION: GITHUB PAGES
1. Sign in or create an account at https://github.com/
2. Create a new public repository, for example "mafia-pass-play".
3. Upload all files and folders inside this package (index.html, manifest.webmanifest, service-worker.js, icons/). Do not upload only the ZIP.
4. In the repository, open Settings → Pages.
5. Under Build and deployment, choose "Deploy from a branch", select the main branch and /(root), then Save.
6. Wait for GitHub Pages to publish the site. Open the HTTPS URL it gives you on your Android phone in Chrome.
7. In Chrome, tap ⋮ → "Install app" or "Add to Home screen" (wording may vary).
8. Launch Mafia from your home screen. Visit once while online so the app files are cached; it can then load offline.

UPDATING
Upload replacement files to the same repository. If you change the app later, increment CACHE_NAME in service-worker.js (for example v2) so devices refresh the cached version.

PRIVACY
The app doesn't send roles or player settings to a server. The service worker only caches the app files from the site where you host it.
