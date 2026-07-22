# SBX Finance v2.33.4 — GitHub Pages Stable Sync

Upload these files to the repository root:

- `index.html`
- `firebase-config.js`
- `.nojekyll`

## What changed

The live Firestore `onSnapshot` UI repaint was disabled. The app still:

- loads the cloud workspace once after login,
- saves local changes immediately,
- pushes changes to Firebase through the existing save queue.

This prevents GitHub Pages from repeatedly replacing the visible page while the user is working.
