# Bharadwaj Celebrations
A buildless, frontend-only planner. All event records and uploaded images live in IndexedDB in the visitor's browser. No analytics, database service or external asset dependencies.

## Vercel
Import this repository, select framework preset Other, leave build command empty and set output directory to dist. Deploy. No environment variables are required.

## Local development
Serve dist with any static HTTP server. Do not open via file://.

## Data
Use Backups to export the complete JSON archive (including images). Import it on the new Vercel origin to migrate records. Different browsers, origins and devices have separate data. Clearing browser storage deletes records. Backups contain private contact information. The last-export date indicates an export was initiated, not proof the user retained the file. No cloud sync or account authentication is included.

Task arrival times use India local time input; display follows the device locale. All event timings except 14 November 2026 18:30 mehendi are intentionally unset.
