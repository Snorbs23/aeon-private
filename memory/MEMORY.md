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

## Recent Articles
| Date | Title | Topic |
|------|-------|-------|
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption, multi-agent systems |

## Recent Digests
| Date | Type | Key Topics |
|------|------|------------|
| 2026-04-06 | Morning Brief | BTC $69K, ETH $2.1K, HYPE token unlock 9.92M tokens ($354M), Gold $4,650/oz |
| 2026-04-06 | DeFi Overview | TVL $94.5B, ETH dominates 57.5%, top yield Jito JitoSOL 5.5% APY |
| 2026-04-06 | Polymarket | Iran ceasefire markets surging; US-Iran deadline extended; Hormuz tensions |
| 2026-04-06 | Token Alert | TRU +135% (pump), RED +70% (unlock+DRILL), WTI Oil $111.81 🚨 (Hormuz) |
| Date | Type | Key Notes |
|------|------|-----------|
| 2026-04-06 | Morning Brief | BTC ~$69k, ETH ~$2.1k, SOL ~$82, HYPE unlock 9.92M tokens |
| 2026-04-06 | DeFi Overview | TVL $94.5B, Ethereum 57.5% dominant, top yield Jito 5.5% |
| 2026-04-06 | Polymarket | US/Iran ceasefire markets surging; "forces enter Iran" 99.7% YES |
| 2026-04-06 | Token Alert | TRU +134%, RED +70%, WTI Oil $111.81 🚨 |
| 2026-03-19 | Changelog | aaronjmars/aeon: 51 commits — dashboard, skills, multi-agent updates |

## Lessons Learned
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging
- aeon.yml has no `schedule` trigger — workflow is dispatch-only (via `workflow_dispatch` or `issues`), so no auto-cron runs

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, token anomalies, WTI Oil/Hormuz, CPI

## Completed Priorities
- Run first morning brief — completed 2026-04-06
- Monitor first token alert — completed 2026-04-06

## Next Priorities
- Wire cron scheduler into aeon.yml to enable scheduled skill runs
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Watch Iran-US situation — could affect Oil/markets (Hormuz tensions)
- CPI due 2026-04-10 — monitor macro impact
- Capture first idea via Telegram (stalled: skill ran twice 2026-04-06 but no idea text provided; needs user to send an idea via Telegram)
- Wire cron scheduler in aeon.yml so daily skills run automatically (currently dispatch-only)
- Add `schedule` cron trigger to `aeon.yml` (open PR) — agent is not autonomous without it
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add morning-brief dedup check (skip if already ran today)
- Add weekly-review and rss-digest to cron once scheduler is wired
- Workflow has no cron schedule — all runs are manual dispatch or message-triggered
- Volume/MC ratio is a reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative

## Next Priorities
- Wire cron schedule to aeon.yml for automated daily runs
- Follow up on HYPE unlock impact (9.92M tokens for Core Contributors)
- Watch CPI print on April 10
- Monitor WTI Oil and Iran ceasefire developments
- Capture Nobu's next idea via Telegram
