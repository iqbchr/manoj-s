# LexisNexis Risk Report - Static Project

This repository contains a single-page static HTML tool that generates a two-page PDF "Risk Management" report from manual input or from an uploaded Excel/CSV file (using the `xlsx`, `html2canvas`, and `jspdf` libraries).

## Files
- `index.html` — the complete app (no build step required).
- `.gitignore` — recommended ignores.
- `LICENSE` — MIT license.

## How to use locally
1. Unzip or clone the repo.
2. Open `index.html` in your browser (Chrome/Edge/Firefox).
3. Fill the form or upload an Excel file with these column headers: `First Name`, `Last Name`, `Gender`, `DOB`, `CaseNo`, `Date`, `Time`.
4. Use **Download Current Report** to save a single PDF or **Generate All PDFs** to create PDFs for every row in the sheet.

## How to upload to GitHub (quick steps)
### Using Git (CLI)
```bash
git init
git add .
git commit -m "Initial commit - LexisNexis Risk Report"
# Create a GitHub repo using the website or `gh` and then:
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

### Or upload via GitHub web UI
1. Create a new repository on GitHub.
2. Click "Add file" → "Upload files" and drop the extracted project files.
3. Commit the changes.

## Notes / Tips
- If the images (logo) do not load due to CORS, try downloading the logo and placing it in the same folder as `index.html` and update the `src` to `./LS_Logo.png`.
- For large Excel files the browser may become slow during PDF generation; split into smaller chunks if needed.

