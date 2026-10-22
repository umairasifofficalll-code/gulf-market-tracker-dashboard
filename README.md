# Gulf Market Tracker

An interactive, three-page dashboard for fictional DFM, ADX, and Tadawul equities from January 2023 to October 2026. Every company, price, and index value is synthetic mock data, not real market information.

## View the dashboard

After GitHub Pages deploys, open: `https://umairasifofficalll-code.github.io/gulf-market-tracker-dashboard/`

The dashboard includes **Market Overview**, **Risk & Return**, and **Stock Detail** pages, with date, sector, exchange, and ticker filters. Green indicates gains; red indicates losses. Risk metrics and correlations use the full available period and do not change with the date filter.

## Data

- `dashboard.json` powers the live dashboard.
- `stocks_dashboard.csv`, `stock_metrics.csv`, and `correlation_long.csv` are prepared for Tableau Desktop or other BI tools.
- `stock_prices_mock.csv`, `stock_info_mock.csv`, and `market_index_mock.csv` are the supplied synthetic source CSVs.
- The three `dashboard_page*_*.png` images are the supplied page references.

The repository includes a browser-viewable dashboard and Tableau-ready data files. It does not include a Tableau `.twb` workbook; the Tableau Desktop window was not accessible to this authoring session.

To regenerate the source tables and dashboard payload, run:

```bash
python scripts/prepare_data.py
python scripts/build_dashboard_data.py
```

The calculation notes and reference layout are described in [the guide](Stock_Market_Dashboard_Guide.docx).
