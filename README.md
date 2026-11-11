# ICONIQ market information and education

Existing npm workspaces: `portal` (React customer app), `admin` (separate React staff console), `server` (Express and persistent SQLite WAL). The conservative release exposes market monitoring where data is authorized, personal watchlists and six original lessons with knowledge checks. Trading, simulated trading, virtual portfolios, financial transfers and investment-service processing are disabled on the server.

```bash
npm ci
npm run build
npm run test:release
npm start
```

Preserve `server/.env` and `server/data/iconiq.db`. Production needs separate strong JWT secrets. Never seed an existing database; the seed command is development-only and explicitly guarded. TradingView’s official hosted widgets display market overviews, prices and charts with attribution. Raw-price APIs remain disabled pending distribution permissions. A selected symbol list supports app search/watchlists; the chart widget provides broader symbol search.

The owner confirmed permission to use ICONIQ and the supplied gold artwork. The transparent wordmark and borderless emblem remain in use.

Android/iPhone use the **hosted VPS application**. Only a looping loading screen is packaged locally; no React application, lessons or offline market pages are bundled. Update the VPS web app to update customer screens. Returning to the mobile app reloads the hosted page. Native changes still require a new binary.

- [Current TradingView widget integration](docs/store-readiness/TRADINGVIEW-WIDGETS.md)
- [Implementation, risks and remaining actions](docs/store-readiness/REPORT.md)
- [Mobile architecture and exact build commands](docs/store-readiness/BUILD-MOBILE.md)
- [Provider permissions](docs/store-readiness/PROVIDERS.md)
- [Store submission and privacy](docs/store-readiness/STORE-SUBMISSION.md)
- [Executed verification](docs/store-readiness/QA.md)
- [Changed files](docs/store-readiness/CHANGED-FILES.md)
- [VPS deployment](DEPLOYMENT-DEMO2.md)

`docs/iconiq/` documents the superseded paper-trading conversion. Its product claims and mobile instructions are historical. `development/simulator/` is unshipped reference code, not a release feature.
