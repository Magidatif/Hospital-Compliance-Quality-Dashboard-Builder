# Hospital Compliance & Quality Dashboard Builder

An interactive, 100% client-side web application built for **Cloudflare Workers (Static Assets)** that converts hospital compliance checklist Excel workbooks (`.xlsx` / `.xls`) into a live executive dashboard.

## Features
- **Instant Excel Parsing**: Reads `BRANCHES ANALYSIS` and checklist sheets (`RAD`, `PH & ST`, `ER`, `OR`, `OUTPAT`, `INPAT`, `ICUS`, `CRASHCART`, `BLOOD BANK`, `LAB`) directly in the browser using SheetJS (`xlsx`).
- **Executive Overview**: KPI cards and interactive Chart.js visualizations for hospital comparisons, active department averages, score distribution, and main category compliance.
- **Heatmap Matrix**: Interactive Hospital × Department compliance matrix with click-to-drill-down filtering.
- **Gaps & Action Plan**: Filterable gap analysis (`0` Not Met, `1` Partially Met, documented notes/corrective actions) with CSV export.
- **Full Checklist Explorer**: Search and filter across all extracted checklist items.
- **Privacy First**: All file parsing runs locally in the browser with zero server uploads.

## Local Development
```bash
npm install
npm run dev
```

## Deploy to Cloudflare
```bash
npx wrangler login
npm run deploy
```
