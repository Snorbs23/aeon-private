# Long-term Memory
*Last consolidated: 2026-04-08*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research
- Cron scheduler is active (skills run on schedule automatically)

## Goals
- Stay on top of AI, crypto, and markets daily
- Build a personal knowledge base over time
- Monitor DeFi positions and market anomalies
- Capture ideas and research as they come

## Recent Articles
| Date | Title | Topic |
|------|-------|-------|
| 2026-04-07 | The Hormuz Chokehold: How the World's Most Critical Oil Lane Became a Powder Keg | Iran-US crisis, oil shock, $200 oil risk |
| 2026-04-07 | Partial Epigenetic Reprogramming: First Human Age-Reversal Trial | Longevity biotech, ER-100, FDA clearance |
| 2026-04-07 | Paper Digest: AI oversight, RegGuard rollups, LLM trading, aging clocks | AI/ML, crypto, markets, health |
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption |
| 2026-04-06 | Self-Review: Quality Audit 2026-04-06 | Agent performance analysis |
| 2026-04-08 | Self-Review: Quality Audit 2026-04-08 | Operational efficiency, 25 heartbeat redundancy, missing cron scheduler |
| 2026-04-07 | The Hormuz Chokehold: How the World's Most Critical Oil Lane Became a Powder Keg | Hormuz crisis, oil shock, Iran-US war, $200 oil, global recession risk |
| 2026-04-07 | Research Brief: Partial Epigenetic Reprogramming (Life Biosciences ER-100, first FDA-cleared age-reversal trial) | Longevity, biohacking, DeSci tokens, AI aging clocks |
| 2026-04-07 | Paper Digest: AI oversight of CUAs, RegGuard rollups, SysTradeBench LLM trading, organ proteomic aging clocks | AI/ML, Crypto, Markets, Longevity |
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption, multi-agent systems |
| 2026-04-06 | Self-Review: Quality Audit 2026-04-06 | Agent quality, noise, gaps, cron scheduler |
| 2026-04-07 | The Hormuz Chokehold | Hormuz crisis, oil shock, Iran-US war, $200 oil risk |
| 2026-04-07 | Research Brief: Epigenetic Reprogramming | Life Biosciences ER-100, first FDA-cleared age-reversal trial |
| 2026-04-07 | Paper Digest | AI CUAs, rollup compliance, LLM trading benchmarks, aging clocks |
| 2026-04-06 | The Age of AI Agents | AI agents, enterprise adoption, multi-agent systems |
| 2026-04-07 | The Hormuz Chokehold | Hormuz crisis, oil shock, Iran-US war, $200 oil, global recession risk |
| 2026-04-07 | Partial Epigenetic Reprogramming: First Human Age-Reversal Trial | Longevity biotech, ER-100, David Sinclair, FDA, DeSci |
| 2026-04-07 | Paper Digest | AI/ML, crypto, markets, health papers |
| 2026-04-06 | The Age of AI Agents | AI agents, enterprise adoption, multi-agent systems |
| 2026-04-06 | Self-Review 2026-04-06 | Agent quality, noise, gaps, cron scheduler |

## Recent Digests
| Date | Type | Key Topics |
|------|------|------------|
| 2026-04-08 | Morning Brief | Iran ceasefire, oil crash to $97 (-14%), BTC $71K (+4%), ETH $2.2K (+7%) |
| 2026-04-07 | Token Alert | BULLA +58%, NOM +26%; TRU -21% reversal; WTI $115 🚨 |
| 2026-04-07 | DeFi Overview | TVL $166.4B, DEX vol +64% ($6.09B), stablecoin contraction |
| 2026-04-07 | Polymarket | Iran ceasefire rejected; US forces enter Iran 99.65% |
| 2026-04-06 | Token Alert | TRU +134%, RED +70%, WTI Oil $111.81/bbl 🚨 |

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, oil shock, Iran crisis
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, thresholds, anomalies

## Lessons Learned
- Volume/MC ratio is reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed
- Pump-dump timing confirmed: TRU +134% → -21% in 1 day; TREE +36% → -15%
- Heartbeat redundancy is major noise: 27 runs in 3 days (needs dedup)
- Idea capture guard now works (prevents empty var runs)
- Iran crisis shifts markets: oil $115→$97 on ceasefire news

## Current Priorities
- **CPI due 2026-04-10** — key macro event in 2 days
- Monitor oil price collapse impact ($97 from $115 peak)
- Track Iran ceasefire stability and market reactions
- Add heartbeat dedup check (critical noise reduction)
- Monitor HYPE post-unlock price action
- Capture first idea via Telegram

## Completed Priorities
- Run first morning brief, token alerts, market monitoring
- Guard idea-capture against empty vars
- Produce quality research (Hormuz article, ER-100 brief)
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging
- aeon.yml has no `schedule` trigger — workflow is dispatch-only (via `workflow_dispatch` or `issues`), so no auto-cron runs
- Volume/MC ratio is a reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative
- Pump-dump cycle timing confirmed: TRU +134% on Apr 6 → -20.8% on Apr 7 (V/MC ratio predicts reversal too)
- Redundant runs are a major noise risk: heartbeat ran 25x in 48h (Apr 6-8); reflect/goal-tracker/self-review each ran 2x — add dedup/guard checks

## Next Priorities
- **[Critical]** Add `schedule` cron trigger to `aeon.yml` (open a PR) — agent is not autonomous without it
- **[Critical]** Add heartbeat dedup check (skip if already ran today) — has run 16 redundant times across 2 days
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add morning-brief dedup check (skip or send price-only update if already ran)
- Monitor CPI print on 2026-04-10 — macro impact on rates and crypto
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Watch WTI Oil and Iran escalation (ceasefire rejected 2026-04-07; $114-115/bbl)
- Add weekly-review and rss-digest to cron once scheduler is wired

## Completed Priorities
- Run first morning brief — completed 2026-04-06
- Monitor first token alert — completed 2026-04-06

## Next Priorities
- **[Critical]** Add `schedule` cron trigger to `aeon.yml` (open a PR) — agent is not autonomous without it  
- **[Critical]** Add heartbeat dedup check (skip if already ran today) — has run 25+ times in 48h
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add morning-brief dedup check (skip or send price-only update if already ran)
- Monitor CPI print on 2026-04-10 — macro impact on rates and crypto
- Monitor WTI Oil and Iran escalation (ceasefire announced 2026-04-08; oil dropped to $97/bbl)
- Add weekly-review and rss-digest to cron once scheduler is wired
- Capture first idea via Telegram (needs Nobu to send an idea via Telegram)
