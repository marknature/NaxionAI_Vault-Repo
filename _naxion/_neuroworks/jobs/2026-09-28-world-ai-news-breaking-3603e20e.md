---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-3603e20e
created: 2026-09-28T08:57:53.650Z
jobId: 3603e20e-e869-490f-9272-fd6e987d9d7e
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-09-28T08:28:24.339Z
finishedAt: 2026-09-28T08:57:52.765Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-09-28T08:28:24.339Z
- **Finished:** 2026-09-28T08:57:52.765Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "chatId": "-1004307136262"
}
```

<details><summary>Log</summary>

```
[2026-09-28T08:28:24.342Z] Sweeping for today's World AI news (RSS + web search).
[2026-09-28T08:28:24.342Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-09-28T08:28:36.956Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-09-28T08:29:32.044Z] [world] web search gathered 14 candidates (quality-filtered).
[2026-09-28T08:29:34.695Z] [history] 19 URLs posted in last 7d
[2026-09-28T08:42:45.439Z] [enrich] arxiv.org 138 → 288 chars
[2026-09-28T08:44:31.756Z] [enrich] desktop.github.com 131 → 462 chars
[2026-09-28T08:50:33.243Z] [enrich] arxiv.org 131 → 289 chars
[2026-09-28T08:57:50.754Z] [quality] scoring skipped: fetch failed — keeping authority-sorted order
[2026-09-28T08:57:51.514Z] [gate] top score 7 < threshold 8 — not breaking enough — queuing as draft, not posting to Telegram
[2026-09-28T08:57:52.765Z] [metrics] world candidates=12 picked=https://arxiv.org/abs/2609.30287 score=7 domains=arxiv.org,github.com,arxiv.org,desktop.github.com,openai.com,ai.google,arxiv.org,arxiv.org
```
</details>
