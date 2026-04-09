# Long-term Memory
*Last consolidated: 2026-04-09*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research
- Cron scheduler is active (skills run on schedule automatically)
- **CRITICAL**: Heartbeat redundancy now at 40+ runs in 4 days (needs immediate dedup fix)

## Goals
- Stay on top of AI, crypto, and markets daily
- Build a personal knowledge base over time
- Monitor DeFi positions and market anomalies
- Capture ideas and research as they come

## Recent Articles
| Date | Title | Topic |
|------|-------|-------|
| 2026-04-09 | The AI Energy Revolution: How Neuro-Symbolic AI Slashed Energy Use by 100x | AI/ML breakthrough, energy efficiency |
| 2026-04-09 | AI-Driven Market Manipulation and Autonomous Trading Agents in 2026 | Research brief, AI trading, market regulation |
| 2026-04-09 | Paper Digest: AI adversarial attacks, Milano 2026 Olympics, olive leaf compounds | AI/ML, health, sports science |
| 2026-04-08 | Self-Review: Quality Audit 2026-04-08 | Operational efficiency, heartbeat redundancy |
| 2026-04-07 | The Hormuz Chokehold: How the World's Most Critical Oil Lane Became a Powder Keg | Iran-US crisis, oil shock |
| 2026-04-07 | Partial Epigenetic Reprogramming: First Human Age-Reversal Trial | Longevity biotech, ER-100 |
| 2026-04-07 | Paper Digest: AI oversight, RegGuard rollups, LLM trading, aging clocks | AI/ML, crypto, markets, health |
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption |
| 2026-04-06 | Self-Review: Quality Audit 2026-04-06 | Agent performance analysis |
| 2026-04-09 | Research Brief: AI-Driven Market Manipulation and Autonomous Trading Agents in 2026 | AI/markets convergence, LLM trading |
| 2026-04-09 | Paper Digest: AI autonomy, female olympians, olive anti-cancer compounds | AI/ML, health research |
| 2026-04-08 | Self-Review: Quality Audit 2026-04-08 | Operational efficiency, 33+ heartbeat redundancy, cron confirmed active |

## Recent Digests
| Date | Type | Key Topics |
|------|------|------------|
| 2026-04-09 | Morning Brief | CPI tomorrow, Iran ceasefire fragile, BTC $71.9K (+4.5%), ETH $2.3K (+6%) |
| 2026-04-09 | Token Alert | NFT sector surge: ENJ +50.7%, BLUR +27.7%, TNSR +31.4%; memes down |
| 2026-04-09 | DeFi Overview | TVL $94.9B, Ethereum 57% dominance, DEX volume stable |
| 2026-04-09 | Polymarket | Iran ceasefire $51.6M volume, sports betting surge (Congo $1.5M) |
| 2026-04-08 | Morning Brief | Iran ceasefire breakthrough, oil crash to $97 (-14%), global rally |
| 2026-04-07 | Token Alert | BULLA +58%, NOM +26%; TRU -21% reversal; WTI $115 🚨 |

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, oil recovery, Iran ceasefire stability, CPI tomorrow
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, NFT surge patterns, volume/MC ratios

## Lessons Learned
- Volume/MC ratio is reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed
- Pump-dump timing confirmed: TRU +134% → -21% in 1 day; TREE +36% → -15%
- Heartbeat redundancy CRITICAL: 33+ runs in 4 days (9+ on 2026-04-09 alone)
- Iran ceasefire breakthrough 2026-04-08: oil crashed $115→$97 (-14%), global rally
- NFT sector surge patterns: ENJ +50.7%, BLUR +27.7%, TNSR +31.4% (2026-04-09)
- Idea capture guard works (prevents empty var runs)
- Cron scheduler IS active (corrected previous "dispatch-only" assessment)

## Current Priorities
- **CPI due 2026-04-10** — key macro event TOMORROW
- Track Iran ceasefire stability (announced 2026-04-08, oil recovering from $97)
- **CRITICAL**: Implement heartbeat dedup (33+ redundant runs in 4 days)
- Monitor NFT sector momentum (ENJ +50.7%, BLUR +27.7% surge detected)
- Monitor HYPE post-unlock price action
- Capture first idea via Telegram

## Completed Priorities
- Run first morning brief, token alerts, market monitoring
- Guard idea-capture against empty vars
- Produce quality research (Hormuz article, ER-100 brief)
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging
- Volume/MC ratio is a reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative
- Pump-dump cycle timing confirmed: TRU +134% on Apr 6 → -20.8% on Apr 7 (V/MC ratio predicts reversal too)
- Redundant runs are a major noise risk: heartbeat ran 25x in 48h (Apr 6-8); reflect/goal-tracker/self-review each ran 2x — add dedup/guard checks
- Redundant runs escalating: heartbeat ran 9x (Apr 6), 11x (Apr 7), 5x+ (Apr 8) — 25+ wasted runs in 3 days
- Morning brief can fail silently: GH Actions showed failure 2026-04-07 02:33 UTC but no error logged
- YAML duplicate keys issue: token-alert defined 3x in aeon.yml but only last entry (4 PM) active; 2 AM/9 AM silently skipped
- Cron scheduler IS active (contrary to earlier "dispatch-only" assessment) — most skills run on schedule


## Next Priorities
- **[Critical]** Add `schedule` cron trigger to `aeon.yml` (open a PR) — agent is not autonomous without it
- **[Critical]** Add heartbeat dedup check (skip if already ran today) — has run 16 redundant times across 2 days
- Guard `idea-capture` against empty `var` to prevent wasted runs
- Add morning-brief dedup check (skip or send price-only update if already ran)
- Monitor CPI print on 2026-04-10 — macro impact on rates and crypto
- Monitor HYPE price action post-unlock (9.92M tokens unlocked 2026-04-06)
- Monitor Iran ceasefire stability (agreement announced 2026-04-08; oil dropped to $97/bbl)
- Add weekly-review and rss-digest to cron once scheduler is wired

## Completed Priorities
- Run first morning brief — completed 2026-04-06
- Monitor first token alert — completed 2026-04-06
- Guard `idea-capture` against empty `var` to prevent wasted runs — completed 2026-04-08

## Next Priorities
- **[Critical]** Add `schedule` cron trigger to `aeon.yml` (open a PR) — agent is not autonomous without it  
- **[Critical]** Add heartbeat dedup check (skip if already ran today) — has run 33+ times in 4 days
- Add morning-brief dedup check (skip or send price-only update if already ran)
- Monitor CPI print on 2026-04-10 — macro impact on rates and crypto
- Monitor WTI Oil and Iran escalation (ceasefire announced 2026-04-08; oil dropped to $97/bbl)
- Add weekly-review and rss-digest to cron once scheduler is wired
- Capture first idea via Telegram (needs Nobu to send an idea via Telegram)
- Run first morning brief, token alerts, market monitoring (2026-04-06)
- Guard idea-capture against empty vars (working as of 2026-04-09)
- Produce quality research (Hormuz article, ER-100 brief, AI energy breakthrough)
- Confirm cron scheduler status (IS active, corrected "dispatch-only" assessment)
- Digest format established: Markdown with clickable links, under 4000 chars
| 2026-04-09 | Morning Brief | CPI tomorrow, oil stabilizing ~$97, BTC $71.9K (+4.5%), ETH $2.25K (+6%) |
| 2026-04-09 | Token Alert | NFT surge (ENJ +50%, BLUR +28%), memes down (FARTCOIN -14%), oil recovery |
| 2026-04-08 | Morning Brief | Iran ceasefire breakthrough, oil crash -14% to $97, global rally |
| 2026-04-07 | Token Alert | BULLA +58%, NOM +26%, TRU reversal -21%, WTI $115 🚨 |
| 2026-04-07 | DeFi Overview | TVL $166.4B, DEX vol surge +64%, stablecoin contraction |

## Topics
- [Markets context](topics/markets.md) — Iran ceasefire resolved, oil collapse, CPI tomorrow
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, current prices, anomalies

## Lessons Learned
- Volume/MC ratio predicts pumps: TRU (13x), RED (4x), TREE (8.5x) all confirmed speculative
- Pump-dump cycle timing: TRU +134% → -21% in 24h; TREE +36% → -15% confirmed
- **CRITICAL**: Heartbeat redundancy escalating: 9x (Apr 6) → 11x (Apr 7) → 8x (Apr 8) → 9x+ (Apr 9)
- Idea capture guard working (prevents empty var runs)
- Iran crisis market impact: oil $115→$97 on ceasefire news, crypto rally +4-7%
- Morning brief can fail silently (GH Actions failure 2026-04-07)
- Cron scheduler IS active for most skills (contrary to earlier "dispatch-only" assessment)

## Current Priorities
- **CPI due 2026-04-10** — critical macro event TOMORROW
- **[CRITICAL]** Add heartbeat dedup check — now 40+ redundant runs in 4 days
- Monitor Iran ceasefire stability and oil price stabilization (~$97)
- Track NFT/gaming token surge pattern (ENJ, BLUR momentum)
- Open cron scheduler PR (still pending despite being flagged for days)

## Completed Priorities
- Iran crisis monitoring (resolved with ceasefire 2026-04-08)
- Quality content production (4 articles + 3 research pieces in 4 days)
- Token anomaly detection (TRU pump-dump cycle successfully predicted)
- Volume/MC ratio validation as pump signal
- Idea-capture empty var guard implementation
