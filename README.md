# C2C Train Times — Thorpe Bay

A lightweight, installable web app showing live c2c train departures to Thorpe Bay from Fenchurch Street and Liverpool Street.

## Features

- **Live departures** — real-time c2c train data from National Rail, filtered specifically for services to Thorpe Bay
- **Station toggle** — switch between Fenchurch Street, Liverpool Street, or view both merged and sorted by departure time
- **Route highlighting** — trains calling at Ockendon, Chafford Hundred, or Grays are marked in red
- **Live countdown** — each departure shows time remaining (e.g. "12 mins time"), updating automatically
- **Delay tracking** — delayed services show the new expected time plus minutes late
- **Full calling points** — tap any train to see every stop with scheduled times down to Thorpe Bay
- **Journey duration** — see total travel time from departure to Thorpe Bay at a glance
- **Auto-refresh** — board updates every 60 seconds, or refresh manually
- **Installable PWA** — add to your home screen on Android for a full app-like experience

## Tech stack

- React 18 (via CDN, no build step)
- Babel Standalone for in-browser JSX transpilation
- [Huxley2](https://github.com/jpsingleton/Huxley2) — a free CORS-enabled proxy for National Rail's Darwin Live Departure Board API
- Single self-contained HTML file — no server, no build tools, no dependencies to install

## Running locally

Just open `thorpe-bay-trains.html` in a browser. No installation needed.

To install as an app on Android:

1. Host the file somewhere reachable (GitHub Pages, Netlify, etc.)
2. Open the URL in Chrome on Android
3. Tap "Add to Home Screen" from the in-app prompt or Chrome's menu

## Data source

Live train data comes from National Rail's Darwin system via the public Huxley2 demo server. As a community-run free service, it has no uptime guarantees — the app falls back to simulated demo data if the live feed is unavailable.

## Author

Leonard Rex