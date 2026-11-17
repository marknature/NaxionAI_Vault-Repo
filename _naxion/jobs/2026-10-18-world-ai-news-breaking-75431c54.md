---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-75431c54
created: 2026-10-18T07:05:12.482Z
jobId: 75431c54-2859-4864-9a9a-326a75792681
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-18T07:00:29.806Z
finishedAt: 2026-10-18T07:05:12.482Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-18T07:00:29.806Z
- **Finished:** 2026-10-18T07:05:12.482Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (6.3s)
2. ✓ Dedupe + enrich — `pipeline` (6.3s)
3. ✓ Quality rank — `pipeline` (47.0s)
4. ✓ Build news card — `pipeline` (282.0s)
5. ✓ Post to Telegram — `pipeline` (282.7s)

## Answer
🧠 DAILY SUPER INTELLIGENCE / AI NEWS — World

Meta removes language that raised scraping and AI training concerns

[TechCrunch AI · 2026-10-17] Meta removes language that raised scraping and AI training concerns
Meta removes language that raised scraping and AI training concerns | TechCrunch {"@context":"https://schema.org","@graph":[{"@type":"NewsArticle","@id":"https://techcrunch.com/2026/10/17/meta-removes-language-that-raised-scraping-and-ai-training-concerns/#article","isPartOf":{"@id":"https://techcrunch

Why it matters


📰 Read more: https://techcrunch.com/2026/10/17/meta-removes-language-that-raised-scraping-and-ai-training-concerns/

#WorldNews #AI #AINews

Source: RSS ≤48h + web search
Story: **Meta removes language that raised scraping and AI training concerns:** [TechCrunch AI · 2026-10-17] Meta removes language that raised scraping and AI training concerns Meta removes language that raised scraping and AI training conc — https://techcrunch.com/2026/10/17/meta-removes-language-that-raised-scraping-and-ai-training-concerns/

<details><summary>Log</summary>

```
[2026-10-18T07:00:29.809Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-18T07:00:29.809Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-18T07:00:35.036Z] [world] web search gathered 15 candidates (quality-filtered).
[2026-10-18T07:00:36.078Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-18T07:00:36.095Z] [history] 42 URLs posted in last 7d
[2026-10-18T07:00:36.095Z] [history] skip already-posted whitehouse.gov
[2026-10-18T07:00:36.095Z] [history] skip already-posted politico.com
[2026-10-18T07:00:36.099Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-10-18T07:00:36.176Z] [enrich] techcrunch.com 96 → 997 chars
[2026-10-18T07:00:36.247Z] [enrich] techcrunch.com 118 → 1019 chars
[2026-10-18T07:00:36.458Z] [enrich] theverge.com 82 → 983 chars
[2026-10-18T07:00:36.461Z] [enrich] theverge.com 87 → 988 chars
[2026-10-18T07:00:36.501Z] [enrich] blogs.nvidia.com 89 → 990 chars
[2026-10-18T07:00:36.991Z] [enrich] techcrunch.com 85 → 986 chars
[2026-10-18T07:01:16.836Z] [quality] scored 12 candidates — top: #2:7 High relevance AI policy change; credibl | #5:7 Significant AI model platform shift; Tec | #3:6 AI hardware news; credible NVIDIA blog; 
[2026-10-18T07:01:16.836Z] Picked 12 fresh candidates (top score 7) — drafting the daily card.
[2026-10-18T07:05:11.804Z] [metrics] world candidates=12 picked=https://techcrunch.com/2026/10/17/meta-removes-language-that-raised-scraping-and-ai-training-concerns/ score=7 domains=techcrunch.com,techcrunch.com,blogs.nvidia.com,techcrunch.com,news.crunchbase.com,energy.gov,switas.com,openvc.app
[2026-10-18T07:05:12.482Z] Posted World BREAKING NEWS to Telegram chat -1004307136262.
```
</details>
