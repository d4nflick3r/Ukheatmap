# UK Postcode Heat Mapper

A static, subscription-free postcode heat map app for Windows or GitHub Pages.

## What it does

- Paste UK postcodes directly into the app.
- Optionally include dates in the pasted rows.
- Create multiple date periods with different colours.
- Show a key / legend for each layer.
- Export the map as a PNG.
- Export plotted point data as CSV.
- Cache postcode lookups in the browser for faster re-use.

## Input formats

These all work:

- `BR8 7RE`
- `2026-03-01, BR8 7RE`
- `BR8 7RE, 01/03/2026`
- `Job123, BR8 7RE, 2026-03-01`
- Tab-separated rows pasted from Excel

## How it works

This app is fully static. There is no backend and no subscription.

For full postcode plotting, the browser calls the free Postcodes.io bulk lookup endpoint and caches results locally in browser storage. That keeps the app GitHub Pages friendly while still allowing accurate full-postcode plotting when online.

## Run locally on Windows

### Simplest method

1. Put the folder anywhere on your PC.
2. Double-click `index.html`.

### Desktop shortcut feel

1. Double-click `Start-UK-Heatmap.bat`.
2. Or create a shortcut to that `.bat` file.

## Publish to GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html` and `README.md`.
3. In the repository settings, enable **Pages**.
4. Set the source to deploy from the main branch root.
5. Open the GitHub Pages URL.

## Notes

- Because the app is static, there is nothing to install on a server.
- Invalid or unresolved postcodes are shown in the summary panel.
- You can host multiple versions by copying the folder into separate repos if needed.
