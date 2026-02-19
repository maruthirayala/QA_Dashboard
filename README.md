# QA Dashboard — Offline v3 (GitHub Pages)

This package is the **offline, no-CDN** build. All libraries are served from `/assets`.

## Structure
```
qa_dashboard_offline_v3/
  index.html
  .nojekyll
  assets/
    README.md
  scripts/
    fetch_assets.sh
    fetch_assets.ps1
```

## Steps to publish
1. Run one of the asset fetch scripts to download **sql-wasm.js**, **sql-wasm.wasm**, **chart.umd.js** into `/assets`.
2. Commit and push everything to your repo (ensure `index.html` is at repo root).
3. In **Settings → Pages**, set **Branch** = `main` (or your default), **Folder** = `/root`.
4. Open your Pages URL and use **Select your SQLite DB**.

> If you see a banner like *"SQL.js not found"* or *"Chart.js not found"*, it means the files are missing from `/assets`.
