# GitHub to Vercel

Extract this archive and open Terminal in the folder that contains vercel.json.

## GitHub
Create an empty private repository named bharadwaj-celebrations at https://github.com/new . Do not initialize a README, license or gitignore there.

Run:

git init -b main
git add .
git commit -m "Initial ceremony planner"
git remote add origin https://github.com/YOUR-USERNAME/bharadwaj-celebrations.git
git push -u origin main

Replace YOUR-USERNAME with your GitHub account or organization. Authenticate using your configured Git credential manager, GitHub CLI, SSH, or a personal access token; account passwords cannot authenticate Git HTTPS pushes. Never put credentials in the project files.

## Vercel
At https://vercel.com/new connect GitHub, grant access to this repository, and import it.
Framework preset: Other
Root directory: ./ (the directory containing vercel.json)
Build command: leave empty (override to empty if necessary)
Output directory: dist
Install command: leave default; no dependencies need installing
Environment variables: none
Deploy, then open the production URL shown by Vercel.

Do not upload the ZIP itself into the repository. Commit the extracted files, keeping dist/ and vercel.json at the root.

## Updates
Edit the files, then:

git add .
git commit -m "Update ceremony planner"
git push

Vercel automatically deploys commits on the connected production branch (main).

## Existing planning data
Export a backup from the original planner and import it via Backups on the Vercel address. Source code does not contain your saved tasks, contacts or images. Every origin/browser/device has its own IndexedDB store. Avoid committing exported backups.

## Local test
With Python 3 installed: python3 -m http.server 8000 --directory dist
Open http://localhost:8000 . No Node dependencies or build step are required.

References:
https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github
https://vercel.com/docs/git
https://vercel.com/docs/builds/configure-a-build
