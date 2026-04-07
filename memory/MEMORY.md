# Long-term Memory
*Last consolidated: 2026-04-07*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research
- **Scheduler note:** `aeon.yml` lacks a `schedule` trigger — only `workflow_dispatch` and `issues`. All runs are manual.

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
| 2026-04-07 | The Hormuz Chokehold: How the World's Most Critical Oil Lane Became a Powder Keg | Hormuz crisis, oil shock, Iran-US war, $200 oil, global recession risk |
| 2026-04-07 | Research Brief: Partial Epigenetic Reprogramming (Life Biosciences ER-100, first FDA-cleared age-reversal trial) | Longevity, biohacking, DeSci tokens, AI aging clocks |
| 2026-04-07 | Paper Digest: AI oversight of CUAs, RegGuard rollups, SysTradeBench LLM trading, organ proteomic aging clocks | AI/ML, Crypto, Markets, Longevity |
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption, multi-agent systems |
| 2026-04-06 | Self-Review: Quality Audit 2026-04-06 | Agent quality, noise, gaps, cron scheduler |
| 2026-04-07 | The Hormuz Chokehold | Hormuz crisis, oil shock, Iran-US war, $200 oil risk |
| 2026-04-07 | Research Brief: Epigenetic Reprogramming | Life Biosciences ER-100, first FDA-cleared age-reversal trial |
| 2026-04-07 | Paper Digest | AI CUAs, rollup compliance, LLM trading benchmarks, aging clocks |
| 2026-04-06 | The Age of AI Agents | AI agents, enterprise adoption, multi-agent systems |

## Recent Digests
| Date | Type | Key Topics |
|------|------|------------|
| 2026-04-06 | Morning Brief | BTC $69K, ETH $2.1K, HYPE token unlock 9.92M tokens ($354M), Gold $4,650/oz |
| 2026-04-06 | DeFi Overview | TVL $94.5B, ETH dominates 57.5%, top yield Jito JitoSOL 5.5% APY |
| 2026-04-06 | Polymarket | Iran ceasefire markets surging; US-Iran deadline extended; Hormuz tensions |
| 2026-04-06 | Token Alert | TRU +135% (pump), RED +70% (unlock+DRILL), WTI Oil $111.81 🚨 (Hormuz) |
| 2026-04-07 | Polymarket | Iran ceasefire Apr 7 deadline failed (4.45% YES); US forces enter Iran Apr 30 at 99.65% |
| 2026-04-07 | DeFi Overview | TVL $166.4B all-chain; DEX vol $6.09B (+64% macro volatility spike); stablecoins -$13.1B |
| 2026-04-07 | Token Alert | Broad risk-off selloff -2-4%; BULLA +58%, NOM +26%; TRU -20.8% (pump reversal confirmed); WTI $115/bbl |
| 2026-03-19 | Changelog | aaronjmars/aeon: 51 commits — dashboard, skills, multi-agent updates |

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, token anomalies, WTI Oil/Hormuz, CPI
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, thresholds, live snapshot, anomalies
| 2026-04-07 | Token Alert | BULLA +58%, NOM +26%, RED +18% (continued); TRU -21% reversal; WTI $115 🚨 |
| 2026-04-07 | DeFi Overview | TVL $166.4B, DEX vol $6.09B (+64%), stablecoins down $13B (redemptions) |
| 2026-04-07 | Polymarket | Iran ceasefire Apr 7 → 4.45% (rejected); "enter Iran by Apr 30" 99.65% YES |
| 2026-04-06 | Morning Brief | BTC $69K, ETH $2.1K, HYPE unlock 9.92M tokens ($354M), Gold $4,650/oz |
| 2026-04-06 | DeFi Overview | TVL $94.5B, ETH 57.5% dominant, top yield Jito JitoSOL 5.5% APY |
| 2026-04-06 | Token Alert | TRU +134%, RED +70%, WTI Oil $111.81/bbl 🚨 (Hormuz disruptions) |

## Lessons Learned
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging
- aeon.yml has no `schedule` trigger — workflow is dispatch-only (via `workflow_dispatch` or `issues`), so no auto-cron runs
- Volume/MC ratio is a reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative
- Pump-dump cycle timing confirmed: TRU +134% on Apr 6 → -20.8% on Apr 7 (V/MC ratio predicts reversal too)
- Redundant runs are a noise risk: heartbeat ran 5x and idea-capture ran 2x (empty var) on 2026-04-06; add dedup/guard checks

- aeon.yml has no `schedule` trigger — workflow is dispatch-only; no auto-cron runs
- Volume/MC ratio is reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative
- Redundant runs are a major noise risk: heartbeat ran 7-9x/day; reflect/goal-tracker/self-review each ran 2x on 2026-04-06 — add dedup/guard checks

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, WTI Oil/Hormuz, CPI
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, thresholds, live snapshot, anomalies

## Completed Priorities
- Run first morning brief — completed 2026-04-06
- Monitor first token alert — completed 2026-04-06

## Next Priorities
- **[Critical]** Add `schedule` cron trigger to `aeon.yml` (open a PR) — agent is not autonomous without it
- **CPI due 2026-04-10** — monitor macro impact on crypto and rates
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Monitor WTI Oil and Iran escalation (deadline passed Apr 7; US forces enter Iran 99.65% YES by Apr 30)
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add heartbeat and morning-brief dedup checks (skip if already ran today)
- Add weekly-review and rss-digest to cron once scheduler is wired
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add heartbeat/morning-brief/reflect dedup checks (skip if already ran today)
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Watch CPI print on 2026-04-10 — key macro event
- Monitor WTI Oil and Iran escalation (ceasefire rejected 2026-04-07; $115/bbl)
- Capture first idea via Telegram (needs Nobu to send an idea via Telegram)
- Add weekly-review and rss-digest to cron once scheduler is wired
