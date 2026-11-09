# Gold Terminal — XAUUSD MVP

A static, browser-based prototype of a technical-analysis terminal for XAUUSD. It is intentionally a **demo-only interface** and does not connect to a broker or provide live market prices.

## Run locally

Open `index.html` in a modern browser, or serve this folder with any static web server. The project can be hosted on GitHub Pages.

## MVP features

- Responsive dark terminal layout and simulated candlesticks
- Timeframe selector, candle/line toggle, chart pan and zoom, fullscreen
- EMA overlays (9/21/50/200), Bollinger Bands and VWAP toggles
- RSI, MACD calculation, ATR readout and a basic candle-pattern scan
- Transparent, rule-based demo summary; illustrative levels only
- Browser notification price alerts and local-only journal

## Data and security

The chart generates random demo candles in the browser. **It is not live XAUUSD data.** Timeframe buttons currently change the display label, not the candle aggregation. Do not use the generated prices, signals, or example levels for trading. A real feed requires an authorized data source and usually a server-side component for credential protection; never put API keys or bot tokens in client-side HTML or a public repository.

The previous version of this repository contained credentials in public source. Replacing the current file does not erase credentials from Git history. Revoke/rotate the exposed API key and Telegram bot token, and remove them from any deployment settings. Add Telegram alerts only through a secure backend.
