# Balance Mensual

A small personal app I use to track my net worth over time: account balances, investments, debts, and money people owe me, with a monthly snapshot and a chart of how it changes.

This is a private tool, not a product. It is shared publicly only because that's how free GitHub Pages hosting works.

## How it works

- `index.html` is the whole app: a single page that installs on a phone like a native app (manifest + service worker).
- The data is **not** in this repository. It lives in a private Google Sheet, reached through a Google Apps Script endpoint that requires a PIN.
- `sw.js` keeps a copy of the app on the device so it opens instantly and works offline.

## Notes

- Please don't try to access the data endpoint; it's rate-limited and locks after repeated wrong PINs.
- Issues and pull requests are not monitored.
