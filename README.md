# Problem 1 (Frontend) – Real-Time Price Ticker
## Description:
Build a simple web page that shows a BTC/USDT ticker updating in real time.

Use HTML/CSS/JS (or React if you prefers).
Fetch price updates from a free API (e.g., Binance or Coinbase REST API) every 5 seconds.

## Display:
- Current price
- % change in last 24 hours
- A green/red indicator depending on price movement since last update.

Deliverables:
- A single-page app (SPA).
- Clean UI (minimal is fine).


# Problem 2 (Frontend) – Mini Order Book UI

## Description:
Build a simple order book table.

Two tables: Buy Orders (bids) and Sell Orders (asks).
Hardcode JSON data (no API required):
```json
{
  "bids": [
    {"price": 61000, "amount": 0.5},
    {"price": 60950, "amount": 1.2}
  ],
  "asks": [
    {"price": 61010, "amount": 0.8},
    {"price": 61020, "amount": 0.3}
  ]
}
```

- Render tables side by side.
- Highlight the best bid and best ask (highest bid, lowest ask).

## Deliverables:
- Responsive table UI.
- Simple sorting logic to always keep best bid/ask on top.

# Problem 3 (Backend) – Trade History API

## Description:
Create a small REST API that simulates trade history.

Use any backend stack (Node.js/Express, Python/FastAPI, Rust/Actix, etc.).

## Provide two endpoints:

- GET /trades → returns all trades in JSON.
- POST /trade → accepts a JSON trade object { "id": 1, "pair": "BTC-USDT", "price": 61000, "amount": 0.5, "side": "buy" } and saves it in memory.

No database needed (in-memory array is fine).
