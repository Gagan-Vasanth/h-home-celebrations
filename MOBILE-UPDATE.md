# Mobile layout update

Replace the dist folder in your existing GitHub working copy with this dist folder. Include the new rosette.svg file. Keep your existing .git folder and remote.

Then run:
git add dist
git commit -m "Fix responsive layouts and iOS decorative icon"
git push

Your connected Vercel project will deploy the push. No build-setting changes are needed. Reload the same production URL once deployment succeeds. CSS and JavaScript references use a new version query to avoid stale cached assets.

Changed: stable vector logo/watermark; phone navigation with all eight sections visible; stacked heading/action and hero/countdown; flexible grids; mobile task rows and budget cards; full-width 16px form inputs; touch targets; safe-area spacing; reduced-motion support.

Browser QA: Chrome iframe widths 320, 390, 430, 600, 768, 900, 1024, 1440. Overview/tasks/budget checked at representative phone/tablet/desktop widths; contacts/moodboard/guests/event-day checked at 390px. No page horizontal overflow detected in those checks. Mobile task save/reopen verified. Real-device iOS Safari and keyboard behavior still need your device check.

Storage schema and IndexedDB database name are unchanged. Existing plans remain on the same origin/browser; do not clear site data. Export a backup before updating as a precaution.
