# DropAlert

DropAlert is a lightweight stock and ETF monitoring web app that alerts users when a selected ticker drops by a user-defined percentage and lets them track portfolio positions and profit/loss.

## Features

- Track stocks and ETFs with custom percentage-drop alerts
- Auto-refresh market data every 60 seconds
- Visual alert banners when a ticker crosses the threshold
- Portfolio tracker with live P&L in dollars and percent
- Light and dark mode
- Responsive design for desktop and mobile

## Run locally

Because this is a static website, you can simply open `index.html` in a browser.

For a cleaner local dev workflow, you can also use a simple server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy on GitHub Pages

1. Create a new GitHub repo.
2. Upload the files from this folder.
3. In GitHub, go to **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/root` folder.
6. Save, then wait for GitHub Pages to publish.

## Notes

- Market data is fetched from Yahoo Finance via a public CORS proxy.
- For production-grade reliability, replace the public proxy with your own backend or a paid market data API.
- Since this is currently a static frontend app, data is stored in memory during the session.

## Suggested next upgrades

- Email alerts
- Push notifications
- User accounts and cloud sync
- Real-time intraday data via Alpaca or Polygon
- Stripe subscription billing
