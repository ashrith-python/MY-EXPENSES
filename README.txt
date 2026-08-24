# My Money — Installable PWA

This folder contains the converted My Money app:

- index.html — your original app, with PWA installation support added
- manifest.json — app name, icon, standalone display, theme
- service-worker.js — offline app shell/cache
- icon.svg / icon-192.png / icon-512.png — app icons

IMPORTANT:
A PWA cannot be installed from a phone by simply opening the HTML as a local
file (file://...). It must be served from HTTPS (or localhost during testing).

For phone installation:
1. Put these files on an HTTPS web host.
2. Open the HTTPS address in Chrome on Android.
3. Chrome should show "Install app" in its menu, or the My Money page will
   show the install (+) button when Chrome exposes the install prompt.
4. Tap Install.

Your transaction data remains in the browser's localStorage, as in the
original HTML app.
