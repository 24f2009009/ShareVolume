# Offline, self-contained Share Outstanding Viewer

This is a production-ready single-page app (SPA) that renders Aon plc's share outstanding using embedded data. No network calls are required. All content is embedded in the HTML file.

Key features:
- Inline CSS/JS only; no external fetches
- data.json content embedded as local data (see data.json in this repo)
- uid.txt content embedded (see uid.txt in this repo)
- Optional ?CIK=10-digit value to swap to an alternate dataset (if provided)
- README.md content is embedded in the page and rendered via markdown parser (marked.js)

Usage:
1) Open index.html
2) Optionally add ?CIK=0001018724 to switch to an alternate dataset (if available in ALTS)
3) Observe the live entity name, max/min values and years updating on the page

Notes:
- This page is designed to be fully self-contained for offline environments.
- The available datasets are embedded in the code (Aon plc as default, and an alternate sample for CIK 0001018724).
