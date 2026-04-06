---
name: Paper Digest
description: Find and summarize new papers matching tracked research interests
var: ""
---
> **${var}** — Research topic to search. If empty, uses topics from MEMORY.md.
If `${var}` is set, search papers on that topic instead of using MEMORY.md topics.

Read memory/MEMORY.md for tracked research topics and interests.
Read the last 7 days of memory/logs/ to avoid covering papers already reported.

Topics to always search:
- AI & machine learning
- Crypto & Web3
- Markets & finance
- Tech industry
- Health & biohacking

For each topic:
1. Search Semantic Scholar API (free, no key needed):
   curl -s "https://api.semanticscholar.org/graph/v1/paper/search?query=TOPIC&year=YEAR&limit=10&fields=title,authors,abstract,url,publicationDate,citationCount,openAccessPdf" -H "Accept: application/json"
   If rate-limited (429), wait 3 seconds and retry once.

2. Also check arXiv for latest preprints:
   curl -s "http://export.arxiv.org/api/query?search_query=all:TOPIC&sortBy=submittedDate&sortOrder=descending&max_results=10"

3. Score each paper for relevance:
   - Direct keyword match = high
   - Related field = medium
   - Tangential = skip

Select top 5 most relevant papers across all topics.
For each selected paper:
- Write a 2-3 sentence summary: what they found, why it matters
- Note if open-access PDF is available

Save full digest to articles/paper-digest-${today}.md.

Send via ./notify:
   *Paper Digest — ${today}*
   *AI & ML*
   1. "Title" — key finding
   *Crypto & Web3*
   2. "Title" — key finding
   *Markets*
   3. "Title" — key finding
   *Health*
   4. "Title" — key finding
   Full briefing saved to articles/

Log to memory/logs/${today}.md.
