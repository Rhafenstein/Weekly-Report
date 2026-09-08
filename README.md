# Reporting Pulse

A self-service dashboard for tracking daily/weekly safety-report submission rates from an iQSMS report-list export — reporting volume by department, whether recent activity is statistically normal, and (when the export includes it) whether average initial risk rating is trending up or down.

**Live version (once GitHub Pages is on):** `https://<your-username>.github.io/<repo-name>/`

## How to use it

1. Open the link above (or just open `index.html` directly in any browser).
2. Drop in your iQSMS report-list export (`.xlsx` or `.csv`) — nothing is uploaded anywhere, it's all processed locally in your browser.
3. Browse the three pages: Overview, Trends & Significance, Risk Trend (if your export has a "Risk level (Initial)" column), and Daily Detail.

To refresh with a new day's numbers, just upload a new export — it's a full cumulative list each time, so the dashboard rebuilds the whole picture from scratch.

## Updating this repo

This is a single self-contained HTML file (`index.html`) — no build step, no dependencies to install. To publish a new version:

1. Replace `index.html` in this repo with the updated file.
2. Commit and push (or use GitHub's "Upload files" button in the web UI to drag-and-drop the replacement).
3. If GitHub Pages is enabled, the live link updates automatically within a minute or two.

## Turning on GitHub Pages (one-time)

Settings → Pages → under "Build and deployment," set Source to "Deploy from a branch," pick your main branch and the `/ (root)` folder → Save. GitHub will give you the live URL a moment later.
