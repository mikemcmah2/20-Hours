# Practice Ledger v2

What's new vs. your first build:
- Starts empty — no default Piano / Hand stands.
- "Manage" link next to the activity wheel lets you remove any activity (its past
  sessions stay logged, just labeled "Removed").
- Adding an activity now asks whether to track **Time**, **Reps**, or **Both**.
- Two separate totals tables: one for time, one for repetitions.
- Uses its own storage keys (`pl2_...`), so it won't collide with v1's data.

## Updating your GitHub repo — overwrite or new repo?

**Overwrite the existing repo (recommended):**
Same install URL, same home-screen icon on your iPad — it just updates in place.
1. Go to your existing repo on github.com (request desktop site in Safari if needed).
2. Tap **Add file → Upload files**.
3. Select these files: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`,
   `icon-512.png`, `icon-512-maskable.png`.
4. GitHub will warn that files with the same names already exist — that's expected,
   it just means they'll be replaced.
5. Scroll down, **Commit changes**.
6. On your iPad, close the installed app fully (swipe it away from the app switcher),
   then reopen it — it should pick up the new version within a minute or so thanks
   to the service worker refresh. If it still looks old, delete the home-screen icon
   and re-add it from Safari.

**Or create a new repo (keeps v1 and v2 separate, side by side):**
Same steps as before — new repo name, upload these files, enable Pages, add to
home screen. You'd end up with two separate app icons and two separate sets of data.

Overwriting is simpler and is what most people want when it's really the same app,
improved. Use a new repo only if you want to keep the old version around too.
