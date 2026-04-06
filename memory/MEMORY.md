# Long-term Memory
*Last consolidated: 2026-04-06*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research

## Goals
- Stay on top of AI, crypto, and markets daily
- Build a personal knowledge base over time
- Monitor DeFi positions and market anomalies
- Capture ideas and research as they come

## Tracked Tokens
| Token | CoinGecko ID | Notes |
|-------|-------------|-------|
| BTC   | bitcoin     | Always show |
| SOL   | solana      | Always show |
| ETH   | ethereum    | Always show |
| HYPE  | hyperliquid | Always show |
| Gold  | n/a         | Use WebSearch |

## Anomaly Thresholds
- Price move: 10%+ in 24h
- Volume spike: 5x+ average
- OI spike: 10%+
- TradFi move: 2%+

## TradFi to Monitor
- Gold, Oil (WTI), 10Y Bond Yield

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

## Skills Built
| Skill | Date | Notes |
|-------|------|-------|

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
