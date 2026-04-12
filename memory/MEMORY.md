# Long-term Memory
*Last consolidated: 2026-04-12*

## About Me
- Name: Nobu
- Location: Bangkok, Thailand (UTC+7)
- Interests: AI & machine learning, Crypto & Web3, Markets & finance, Tech industry news, Health & biohacking

## About This Repo
- Autonomous agent running on GitHub Actions via Claude Code
- Sends daily briefings, monitors markets, writes articles and research
- Cron scheduler is active (skills run on schedule automatically)
- **CRITICAL**: Heartbeat redundancy now at 40+ runs in 4 days (needs immediate dedup fix)
- **CRITICAL:** Workflow is dispatch-only - NO cron scheduler configured
- **Heartbeat redundancy:** 50+ runs in 4 days, needs deduplication

## Goals
- Stay on top of AI, crypto, and markets daily
- Build a personal knowledge base over time
- Monitor DeFi positions and market anomalies
- Capture ideas and research as they come

## Recent Articles
| Date | Title | Topic |
|------|-------|-------|
| 2026-04-12 | Multi-Agent AI Orchestration: The Infrastructure Revolution of 2026 | Research brief, AI orchestration, enterprise systems |
| 2026-04-12 | Paper Digest: DMax diffusion, DISCO protein design, biological coordination | AI/ML, biotech, health research |
| 2026-04-11 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | Research brief, AI agents, enterprise adoption |
| 2026-04-11 | Paper Digest: Meta-cognitive AI, MEV-ACE, MonoUNet knee cartilage | AI/ML, crypto, health research |
| 2026-04-10 | The Great Inflation Reversal of 2026 - CPI Data and Iran War Market Disruption | Research brief, inflation, macro |
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
| 2026-04-09 | Self-Review: Quality and Reliability Audit 2026-04-09 | Critical infrastructure gap, 75% inefficiency, missing cron scheduler |
| 2026-04-09 | The AI Energy Revolution: How Neuro-Symbolic AI Slashed Energy Use by 100x | AI/ML breakthrough, energy efficiency, Tufts University |
| 2026-04-09 | Research Brief: AI-Driven Market Manipulation and Autonomous Trading Agents | AI trading, market manipulation, regulatory frameworks |
| 2026-04-09 | Paper Digest: Claudini attacks, Olympic performance, olive cancer compounds | AI/ML, health, crypto, markets research |
| 2026-04-08 | Self-Review: Quality Audit 2026-04-08 | Operational efficiency, heartbeat redundancy |
| 2026-04-07 | The Hormuz Chokehold: How the World's Most Critical Oil Lane Became a Powder Keg | Iran-US crisis, oil shock, $200 oil risk |
| 2026-04-07 | Research Brief: Partial Epigenetic Reprogramming | Longevity biotech, ER-100, FDA clearance |
| 2026-04-07 | Paper Digest: AI oversight, RegGuard rollups, LLM trading, aging clocks | AI/ML, crypto, markets, health |
| 2026-04-06 | The Age of AI Agents: How Autonomous Software Is Reshaping Work in 2026 | AI agents, enterprise adoption |
| 2026-04-06 | Self-Review: Quality Audit 2026-04-06 | Agent performance analysis |

## Recent Digests
| Date | Type | Key Topics |
|------|------|------------|
| 2026-04-12 | Token Alert | OKZOO +201% (AI surge), TrueFi +63%, core crypto down 1-3% |
| 2026-04-12 | DeFi Overview | TVL $95.5B (+0.6%), Ethereum 56.7% dominance, stable consolidation |
| 2026-04-11 | Token Alert | IoTeX +264.81%, Flamingo +112.98% major pumps; post-CPI rally |
| 2026-04-11 | Polymarket | Fed rate markets dominate $5.8M volume; Iran volume collapsed post-CPI |
| 2026-04-10 | Polymarket | Iran ceasefire $54.4M volume despite resolution, VP Vance talks Pakistan |
| 2026-04-10 | Research Brief | CPI inflation reversal, Iran war market disruption, crypto binary move |
| 2026-04-09 | Morning Brief | CPI tomorrow, Iran ceasefire fragile, BTC $71.9K (+4.5%), ETH $2.3K (+6%) |
| 2026-04-09 | Token Alert | NFT sector surge: ENJ +50.7%, BLUR +27.7%, TNSR +31.4%; memes down |
| 2026-04-09 | DeFi Overview | TVL $94.9B, Ethereum 57% dominance, DEX volume stable |
| 2026-04-09 | Polymarket | Iran ceasefire $51.6M volume, sports betting surge (Congo $1.5M) |
| 2026-04-08 | Morning Brief | Iran ceasefire breakthrough, oil crash to $97 (-14%), global rally |
| 2026-04-07 | Token Alert | BULLA +58%, NOM +26%; TRU -21% reversal; WTI $115 🚨 |

## Topics
- [Markets context](topics/markets.md) — geopolitical macro, oil recovery, Iran ceasefire stability, CPI tomorrow
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, NFT surge patterns, volume/MC ratios
- [Markets context](topics/markets.md) — geopolitical macro, oil shock, Iran crisis
- [Market monitoring](topics/market-monitoring.md) — tracked tokens, thresholds, anomalies

## Lessons Learned
- **ROOT CAUSE FOUND**: Heartbeat redundancy caused by missing schedule triggers in GitHub Actions workflow
- AI token surge patterns: OKZOO +200%, ARIA +60%, SkyAI +37% (2026-04-12)
- Volume/MC ratio is reliable pump signal: TRU (13x), RED (4x), TREE (8.5x) all confirmed
- Pump-dump timing confirmed: TRU +134% → -21% in 1 day; TREE +36% → -15%
- Major pump signals: IoTeX +264.81%, Flamingo +112.98% (2026-04-11)
- CPI result drives market focus shift: geopolitical → monetary policy
- Iran ceasefire breakthrough 2026-04-08: oil crashed $115→$97 (-14%), global rally
- Idea capture guard works (prevents empty var runs)

## Current Priorities  
- **CRITICAL**: Fix GitHub Actions workflow - missing schedule triggers (root cause of redundancy)
- **Monitor**: AI token rotation patterns (OKZOO +200%+, multiple 30%+ gainers)
- **Monitor**: Market shift from geopolitical (Iran) to monetary policy (Fed rates) 
- **Post-CPI monitoring**: 3.3% result triggered Fed rate market activity
- Monitor DeFi stability (TVL $95.5B, consolidation phase)
- Capture first idea via Telegram

## Completed Priorities  
- Run first morning brief, token alerts, market monitoring
- Guard idea-capture against empty vars
- Produce quality research (Hormuz article, ER-100 brief, AI energy revolution)
- Digest format: Markdown with clickable links, under 4000 chars
- Always save files AND commit before logging


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
- **[URGENT]** Add cron scheduler to `.github/workflows/aeon.yml` — no scheduled skills running
- **[CRITICAL]** Add heartbeat dedup check — 50+ redundant runs in 4 days 
- **[HIGH]** Fix YAML duplicate token-alert keys (only 4 PM slot active)
- Monitor CPI data release 2026-04-10 — major macro event tomorrow
- Monitor Iran ceasefire stability and oil price recovery ($97 from $115)
