---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-53a91b26
created: 2026-11-02T07:00:37.470Z
jobId: 53a91b26-e8e2-40de-8e0d-70e53f348630
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-02T07:00:18.498Z
finishedAt: 2026-11-02T07:00:37.469Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-02T07:00:18.498Z
- **Finished:** 2026-11-02T07:00:37.469Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (8.9s)
2. ✓ Dedupe + enrich — `pipeline` (9.0s)
3. ✓ Quality rank — `pipeline` (16.6s)
4. ✓ Build news card — `pipeline` (18.2s)
5. ✓ Post to Telegram — `pipeline` (19.0s)

## Answer
🧠 DAILY SUPER INTELLIGENCE / AI NEWS — World

Trump orders renaming AI as “super intelligence” in PubMed

US President Donald Trump has issued an order titled _Inaugurating the Era of Super Intelligence_, directing federal agencies to replace the terms “artificial intelligence” and “AI” with “Super Intelligence” and “SI.” The change is already being implemented in PubMed, the world’s leading biomedical literature database. The order applies to all official communications, websites, reports, and policy documents. Scientists have criticized the move.

Why it matters


📰 Read more: https://www.bmj.com/content/395/bmj-2026-101244

#WorldNews #AI #AINews #SuperIntelligence #PubMed #TechPolicy

Source: RSS ≤48h + web search
Story: **Trump orders renaming AI as “super intelligence” in PubMed:** 3. Trump orders renaming AI as “super intelligence” in PubMed # Trump orders renaming AI as “super intelligence” in PubMed Scientists have criticised US presid — https://www.bmj.com/content/395/bmj-2026-101244

<details><summary>Log</summary>

```
[2026-11-02T07:00:18.509Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-02T07:00:18.509Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-02T07:00:25.288Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-02T07:00:27.443Z] [world] web search gathered 14 candidates (quality-filtered).
[2026-11-02T07:00:27.467Z] [history] 107 URLs posted in last 7d
[2026-11-02T07:00:27.468Z] [history] skip already-posted nextgov.com
[2026-11-02T07:00:27.468Z] [history] skip already-posted whitehouse.gov
[2026-11-02T07:00:27.472Z] [filter] deduped 22 → 20 (spam/history removed)
[2026-11-02T07:00:28.067Z] [enrich] arxiv.org 142 → 1043 chars
[2026-11-02T07:00:28.287Z] [enrich] arxiv.org 106 → 1007 chars
[2026-11-02T07:00:28.290Z] [enrich] arxiv.org 119 → 1020 chars
[2026-11-02T07:00:28.928Z] [enrich] arxiv.org 113 → 1014 chars
[2026-11-02T07:00:29.961Z] [enrich] arxiv.org 117 → 1018 chars
[2026-11-02T07:00:30.475Z] [enrich] arxiv.org 146 → 1047 chars
[2026-11-02T07:00:35.110Z] [quality] scored 12 candidates — top: #9:8 High impact political directive affectin | #12:8 High relevance; major tech CEOs adopting | #3:6 Relevant protocol for LLM fairness, thou
[2026-11-02T07:00:35.110Z] Picked 12 fresh candidates (top score 8) — drafting the daily card.
[2026-11-02T07:00:36.706Z] [metrics] world candidates=12 picked=https://www.bmj.com/content/395/bmj-2026-101244 score=8 domains=bmj.com,cnbc.com,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-02T07:00:37.468Z] Posted World BREAKING NEWS to Telegram chat -1004307136262.
```
</details>
