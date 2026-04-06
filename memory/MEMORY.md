# Long-term Memory
*Last consolidated: 2026-04-06*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research
- **Scheduler note:** Workflow (`aeon.yml`) lacks a `schedule` trigger — only `workflow_dispatch` and `issues`. Skills run on demand only, no automated cron.

## Goals
- Stay on top of AI, crypto, and markets daily
- Build a personal knowledge base over time
- Monitor DeFi positions and market anomalies
- Capture ideas and research as they come

## Market Monitoring
See [memory/topics/market-monitoring.md](topics/market-monitoring.md) for tokens, thresholds, and latest snapshot.
See [memory/topics/markets.md](topics/markets.md) for geopolitical macro and event context.

## Recent Articles
| Date | Title | Topic |
|------|-------|-------|
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption, multi-agent systems |

## Recent Digests (2026-04-06)
| Type | Key Notes |
|------|-----------|
| Morning Brief | BTC $69K, ETH $2.1K, HYPE unlock 9.92M tokens ($354M), Gold $4,650/oz |
| DeFi Overview | TVL $94.5B, Ethereum 57.5% dominant, top yield Jito JitoSOL 5.5% APY |
| Polymarket | US/Iran ceasefire markets surging; "forces enter Iran by Apr 30" 99.7% YES |
| Token Alert | TRU +134%, RED +70%, WTI Oil $111.81/bbl 🚨 (Hormuz disruptions) |

## Lessons Learned
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging
- aeon.yml has no `schedule` trigger — workflow is dispatch-only; no auto-cron runs
- Volume/MC ratio is a reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative

## Completed Priorities
- Run first morning brief — completed 2026-04-06
- Monitor first token alert — completed 2026-04-06

## Next Priorities
- Add `schedule` cron trigger to `aeon.yml` (open PR) — agent is not autonomous without it
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Watch Iran-US situation — could affect Oil/markets (Hormuz tensions)
- CPI due 2026-04-10 — monitor macro impact
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add morning-brief dedup check (skip if already ran today)
- Add weekly-review and rss-digest to cron once scheduler is wired
