# Practice Ledger — PWA

A installable app for tracking time spent on practice activities. Uses `localStorage`,
so data stays on the device and survives closing the app, unlike the Claude artifact version.

## Files
- `index.html` — the app
- `manifest.json` — makes it installable
- `sw.js` — service worker, lets it work offline once installed
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — app icons

## Fastest way to get this on your iPad (free, no Mac needed)

**1. Host the files** (GitHub Pages is free and simple):
   - Create a free GitHub account if you don't have one.
   - Create a new repository (e.g. `practice-ledger`).
   - Upload all 5 files in this folder to the repo (use "Add file" → "Upload files" on github.com — no command line needed).
   - Go to the repo's **Settings → Pages**, set source to the `main` branch / root folder, and save.
   - GitHub gives you a URL like `https://yourusername.github.io/practice-ledger/`.

**2. Install it on your iPad:**
   - Open that URL in **Safari** on the iPad (must be Safari, not Chrome).
   - Tap the **Share** icon (square with an arrow).
   - Tap **Add to Home Screen**.
   - It now appears as an app icon and opens full-screen with no browser bar.

**3. That's it.** Data is stored locally in that installed app via `localStorage` and
   will still be there after force-quitting, restarting the iPad, or going offline.

## Notes
- Data does **not** sync between devices or between the home-screen app and Safari itself —
  it's local to that one installed instance. If you want cross-device sync later, that
  would need a real backend/database, which is a bigger step up from this.
- If you ever want to back up your data, you can open Safari's developer tools or ask me
  to add an export/import button to this version too.
