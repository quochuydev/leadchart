# Crypto and AI Agent

## index.html — BTC vs XAU Lead-Lag Chart

A single-file dashboard deployed on GitHub Pages that visualizes the **lead-lag relationship** between Bitcoin (BTC) and Gold (XAU/PAXG).

**Concept:** BTC is believed to lead gold by N days. By showing BTC's older price movement alongside XAU's recent movement — both normalized to % change from their start — you can visually test whether BTC's pattern preceded XAU's.

**How it works:**
- BTC: fetches 200 daily candles, displays the oldest N (configurable)
- XAU: fetches 100 daily candles, displays all 100 (the recent period)
- Both lines start at 0% — y-axis shows % change from each line's first candle
- Adjust **BTC lead days** input (default 100) to shift how many BTC candles are shown

**Data source:** Binance public API (`BTCUSDT`, `PAXGUSDT` daily klines)
