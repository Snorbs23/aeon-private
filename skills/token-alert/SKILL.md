---
name: Token Alert
description: Notify on price or volume anomalies for tracked tokens
var: ""
---
> **${var}** — Token symbol or CoinGecko ID. If empty, checks all tracked tokens.
If `${var}` is set, only check that token.

Read memory/MEMORY.md for tracked tokens and alert thresholds.
Read the last 2 days of memory/logs/ for previous prices to detect changes.

Steps:
1. Always fetch and display current prices for core tokens:
   - BTC (bitcoin), SOL (solana), ETH (ethereum), HYPE (hyperliquid), Gold (XAU)
   - Use CoinGecko for crypto, use WebSearch for Gold price
   - Show: current price + 24h % change + 24h volume

2. Scan market-wide for anomalies (top 200 coins by volume):
   - Flag ANY coin with 10%+ price move in 24h (up or down)
   - Flag ANY coin with volume spike 5x+ above its average
   - Flag ANY coin with OI spike 10%+ (use WebSearch for OI data)
   - Flag daily top gainers and losers
   - For TradFi: use WebSearch to check Gold, Oil (WTI), Bonds (10Y yield) for 2%+ moves

3. Format and send via ./notify:
   *Token Alert — ${today}*

   *Core Prices*
   - BTC: $X (+X%) Vol: $X
   - SOL: $X (+X%) Vol: $X
   - ETH: $X (+X%) Vol: $X
   - HYPE: $X (+X%) Vol: $X
   - Gold: $X (+X%)

   *🚨 Anomalies (10%+ moves only)*
   - TOKEN: $X (+X% 24h) — price spike
   - TOKEN: volume spike Nx average
   - TOKEN: OI spike X%

   *📈 Top Gainers (24h)*
   - TOKEN: +X%
   - TOKEN: +X%

   *📉 Top Losers (24h)*
   - TOKEN: -X%
   - TOKEN: -X%

   *📊 TradFi*
   - Gold: $X (+X%)
   - Oil: $X (+X%)
   - 10Y Yield: X% (+X%)

4. Log all prices to memory/logs/${today}.md.
If no anomalies detected, still send core prices and log "TOKEN_ALERT_OK".
