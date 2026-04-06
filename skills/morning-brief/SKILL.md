---
name: Morning Brief
description: Aggregated daily briefing — digests, priorities, and what's ahead
var: ""
---
> **${var}** — Area to emphasize. If empty, covers all areas.
If `${var}` is set, emphasize that area in the briefing.
Read memory/MEMORY.md for goals, priorities, and tracked items.
Read yesterday's and today's memory/logs/ entries.
Steps:
1. Gather inputs:
   - **Priorities**: top 3 items from MEMORY.md "Next Priorities"
   - **Yesterday's activity**: summarize what Aeon did yesterday from logs
   - **Pending items**: any stalled PRs, unresolved alerts, or open issues from recent logs
   - **Scheduled today**: check aeon.yml for what skills run today
2. Check for headlines across these topics:
   - AI & machine learning
   - Crypto & Web3
   - Markets & finance
   - Tech industry news
   - Health & biohacking
   - Use WebSearch for 2-3 top headlines per topic
   - Keep headlines to one line each
3. Check prices and include in brief:
   - BTC, SOL, ETH, HYPE, Gold — current price + 24h % change
4. Format and send via `./notify`:
