# Plutus Dashboard Weekly Tables

This project is a lightweight dashboard built from the same architecture as `Plutus_dashboard`:

- Static `index.html` UI
- Netlify function at `/.netlify/functions/data` for CSV proxy + cache
- Scheduled Netlify refresh function

## Data source

By default the functions use:

`https://data.testbook.com/api/queries/22270/results.csv?api_key=rasXttOaulP2b09edlGAVbS57YNItF8jJLAntnkH`

You can override with Netlify env var:

`UPSTREAM_URL=<your_csv_url>`

## Implemented

- Source filter with **Total** chip to select all sources at once
- Week filter with **Total** chip to select all weeks at once
- Two weekly metric tables (Week 1 to Week 4) exactly as requested
