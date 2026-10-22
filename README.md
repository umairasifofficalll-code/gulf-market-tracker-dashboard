# Gulf Market Tracker

An interactive, three-page dashboard for fictional DFM, ADX, and Tadawul equities from January 2023 to October 2026. Every company, price, and index value is synthetic mock data, not real market information.

## View the dashboard

The GitHub Pages site is being deployed at: `https://umairasifofficalll-code.github.io/gulf-market-tracker-dashboard/`

The dashboard includes **Market Overview**, **Risk & Return**, and **Stock Detail** pages with date, sector, exchange, and ticker filters. Green indicates gains; red indicates losses. Risk metrics and correlations use the full available period and do not change with the date filter.

## Repository contents

- `index.html` and `dashboard.json` power the browser dashboard.
- `stocks_dashboard.csv`, `stock_metrics.csv`, and `correlation_long.csv` are prepared for Tableau Desktop and other BI tools.
- `stock_prices_mock.csv`, `stock_info_mock.csv`, and `market_index_mock.csv` are the synthetic source files.
- `Stock_Market_Dashboard_Guide.docx` and the three `dashboard_page*_*.png` files are the supplied guide and page references.
- `.github/workflows/pages.yml` deploys the site to GitHub Pages on pushes to `main`.

The repository includes a browser-viewable dashboard and Tableau-ready data files. It does not include a native Tableau `.twb` workbook because Tableau Desktop was not accessible to the authoring session.
