# Sweep Desk

BTC spot swing decision desk. It marks liquidity pools, checks whether a sweep reclaimed, and calls long or short. It does not place orders.

Spot can only buy. A short call means stay out or reduce a long you already hold.

Open `index.html` in a browser. Refresh loads BTC-USDT candles from OKX. Type the latest ETF flow, funding, and open-interest change. The call updates as you edit.

## Calls

- LONG: lows swept, 4-hour close back above, up displacement. Buy the retest.
- SHORT: highs swept, close back below, down displacement. Not a spot order.
- SHORT BIAS: a low broke and was not reclaimed. Do not buy the bounce.
- FLAT: no qualified sweep.

Two ETF outflow days lean short. Two inflow days lean long. Funding above 0.03% per 8 hours blocks a fresh long. Funding below −0.03% blocks a fresh short.

This is a checklist, not a signal service.
