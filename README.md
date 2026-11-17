# Process Capability Analyzer

Web tool that calculates Cp, Cpk, Pp and Ppk, draws histograms and control charts,
summarises characteristics that are not capable, and suggests how to reach the Cpk target.
Accepts PDF inspection/CMM reports, Excel and CSV files.

Pure static site (HTML + JavaScript, libraries loaded from cdnjs) — no build step.

## Run locally
Open the folder in VS Code, right-click `index.html` → **Open with Live Server**.

## Deploy
Hosted on **Azure Static Web Apps** (Free plan). Every push to `main` redeploys
automatically through the GitHub Actions workflow that Azure adds to `.github/workflows/`.

Azure build settings: App location `/`, API location *(empty)*, Output location *(empty)*.

## Files
- `index.html` – the whole app
- `staticwebapp.config.json` – Azure Static Web Apps routing
- `samples/` – example PDF reports for testing
