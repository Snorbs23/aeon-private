---
name: DeFi Overview
description: Daily DeFi anomalies and movers — TVL changes, unusual activity, emerging protocols
var: ""
---
> **${var}** — Chain or protocol to focus on. If empty, shows full overview.

Read memory/MEMORY.md for context.
Read the last 2 days of memory/logs/ to compare against yesterday's data.

Steps:
1. Fetch DeFi data:
   curl -s "https://api.llama.fi/v2/chains"
   curl -s "https://api.llama.fi/protocols"
   curl -s "https://api.llama.fi/overview/dexs?excludeTotalDataChart=true&excludeTotalDataChartBreakdown=true"
   curl -s "https://stablecoins.llama.fi/stablecoins?includePrices=false"
   curl -s "https://yields.llama.fi/pools" | jq '[.data | sort_by(-.tvlUsd) | .[:20] | .[] | {project, chain, symbol, tvlUsd, apy}]'

2. Focus on what's UNUSUAL and MOVING — skip anything stable or obvious:
   - Chains or protocols with 10%+ TVL change in 24h
   - Any protocol outside top 20 suddenly spiking into top 10
   - Unusual DEX volume spikes (2x+ normal)
   - Stablecoin supply sudden increase or decrease
   - New high-yield pools that appeared in last 24h with >$10M TVL
   - Compare against yesterday's log — flag anything that shifted significantly

3. Send via ./notify:
   *DeFi Anomalies — ${today}*

   *Total TVL:* $X.XXB (±
