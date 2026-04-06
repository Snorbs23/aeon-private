---
name: Daily Article
description: Research trending topics and write a publication-ready article
var: ""
---
> **${var}** — Topic to write about. If empty, auto-selects a trending topic.
If `${var}` is set, write about that topic instead of auto-selecting.

Today is ${today}. Your task is to research and write a high-quality article.

Topics to focus on:
- AI & machine learning
- Crypto & Web3
- Markets & finance
- Tech industry news
- Health & biohacking

Steps:
1. Read memory/MEMORY.md for context on what topics have been covered recently.
2. Search the web for the most interesting recent developments across the above topics — pick whichever has the most compelling story today. Use WebSearch to find current sources.
3. Read 2-3 source articles to gather facts using WebFetch.
4. Write a 600-800 word article in markdown. Include:
   - A compelling title
   - A short intro hook
   - 3-4 substantive sections
   - Cited sources at the bottom
5. Save the article to: articles/${today}.md
6. Update memory/MEMORY.md to record the article topic.
7. Log what you did to memory/logs/${today}.md.
8. Send via ./notify: "New article written: [title]\n\nhttps://github.com/${repo}/blob/main/articles/${today}.md"

Write complete, publication-ready content. No placeholders.
