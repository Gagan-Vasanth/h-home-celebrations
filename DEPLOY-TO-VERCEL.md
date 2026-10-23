# Deploy Bharadwaj Celebrations to Vercel

1. Extract this ZIP.
2. Open Terminal in the extracted folder containing vercel.json.
3. With Node.js installed, run: npx vercel --prod
4. Sign into Vercel and create a project when prompted.
5. Use Framework Preset: Other, no build command, Output Directory: dist.

Alternative: upload the extracted files to a GitHub repository and import that repository into Vercel with the same settings. Keep dist/ and vercel.json at the repository root.

No environment variables, database, API keys or application dependencies are needed.
This ZIP contains source files, not browser-saved planning data.
To migrate your existing plan, export a backup from the old site, then restore it through Backups on the new Vercel site. Each site address/browser/device has separate storage.

Documentation: https://vercel.com/docs/cli/deploy
