---
name: Research Brief
description: Deep dive on a topic combining web search, papers, and synthesis
var: ""
---
> **${var}** — Topic to research. Recommended for best results.
If `${var}` is set, use it as the research topic.

If no topic given, auto-select the most interesting current development from:
- AI & machine learning
- Crypto & Web3
- Markets & finance
- Tech industry news
- Health & biohacking

Read memory/MEMORY.md for context on prior research and interests.

Steps:
1. Use WebSearch to find 5-8 current sources on the topic.
2. Search Semantic Scholar for relevant academic papers:
   curl -s "https://api.semanticscholar.org/graph/v1/paper/search?query=TOPIC&limit=10&fields=title,authors,abstract,url,publicationDate,citationCount,openAccessPdf"
3. Use WebFetch to read the 3-4 most relevant sources in depth.
4. Synthesize a research brief (600-1000 words):
   - Overview — what this topic is and why it matters now
   - Current state — what's known, key players, recent developments
   - Key papers — 2-3 most relevant papers with summaries
   - Open questions — what's unresolved or emerging
   - Connections — how this relates to topics in MEMORY.md
5. Save to articles/research-brief-${today}.md.
6. Send abbreviated summary via ./notify.
7. Log what you did to memory/logs/${today}.md.
