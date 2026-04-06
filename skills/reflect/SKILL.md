---
name: Weekly Reflect
description: Review recent activity, consolidate memory, and prune stale entries
var: ""
---
> **${var}** — Area to focus on. If empty, reviews everything.
If `${var}` is set, focus the reflection on that specific area.

Today is ${today}. Review recent activity and maintain long-term memory.

Steps:
1. Read memory/MEMORY.md to understand current memory state.
2. Read memory/logs/ for the last 7 days.
3. Read articles/ for the last 7 days.
4. Consolidate:
   - What topics have been covered? Note patterns or gaps.
   - What was built or created?
   - Any stale entries in MEMORY.md? Remove them.
   - Any recurring errors worth noting?
5. Reorganize memory:
   - Keep MEMORY.md as a short index (~50 lines)
   - Move detailed notes into memory/topics/ files
   - Update existing topic files rather than creating new ones
6. Log what you did to memory/logs/${today}.md.
7. Send via ./notify: "Memory consolidated — ${today}"

Be ruthless about pruning. Memory should be useful, not an append-only log.
