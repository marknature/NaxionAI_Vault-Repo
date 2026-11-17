---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-d2c2fe4c
created: 2026-10-28T19:35:04.711Z
jobId: d2c2fe4c-8d0e-4522-9b25-ac7b25878d9e
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-28T19:11:50.610Z
finishedAt: 2026-10-28T19:35:04.711Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-10-28T19:11:50.610Z
- **Finished:** 2026-10-28T19:35:04.711Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "chatId": "<existing>",
  "videoUrl": "<existing>"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (8.9s)
2. ✓ Dedupe + enrich — `pipeline` (8.9s)
3. ✓ Quality rank — `pipeline` (358.7s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-28T19:11:50.611Z] Queued — 1 task ahead (cap 2 running at once).
[2026-10-28T19:29:06.039Z] Started after 1035s in the task queue.
[2026-10-28T19:29:06.039Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-28T19:29:06.039Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-28T19:29:11.271Z] [africa] web search gathered 18 candidates (quality-filtered).
[2026-10-28T19:29:14.924Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-10-28T19:29:14.955Z] [history] 92 URLs posted in last 7d
[2026-10-28T19:29:14.956Z] [history] skip already-posted daily.dev
[2026-10-28T19:29:14.956Z] [history] skip already-posted daily.dev
[2026-10-28T19:29:14.956Z] [history] skip already-posted daily.dev
[2026-10-28T19:29:14.956Z] [history] skip already-posted daily.dev
[2026-10-28T19:29:14.956Z] [history] skip already-posted daily.dev
[2026-10-28T19:29:14.956Z] [history] skip already-posted facebook.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted qz.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted iafrica.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted reuters.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted ainowinstitute.org
[2026-10-28T19:29:14.956Z] [history] skip already-posted facebook.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted dlapiper.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted africatechsummit.com
[2026-10-28T19:29:14.956Z] [history] skip already-posted africatechfestival.com
[2026-10-28T19:29:14.960Z] [filter] deduped 26 → 12 (spam/history removed)
[2026-10-28T19:29:16.687Z] [enrich] techcabal.com 93 → 994 chars
[2026-10-28T19:29:16.813Z] [enrich] techcabal.com 93 → 994 chars
[2026-10-28T19:29:16.967Z] [enrich] techcabal.com 95 → 996 chars
[2026-10-28T19:29:17.096Z] [enrich] iafrica.com 128 → 1029 chars
[2026-10-28T19:29:17.191Z] [enrich] techcabal.com 100 → 1001 chars
[2026-10-28T19:29:17.816Z] [enrich] iafrica.com 97 → 998 chars
[2026-10-28T19:35:04.706Z] [quality] scoring skipped: Unexpected non-whitespace character after JSON at position 123 (line 2 column 1) — keeping authority-sorted order
[2026-10-28T19:35:04.707Z] [gate] top score 7 < threshold 8 — not breaking enough — queuing as draft, not posting to Telegram
[2026-10-28T19:35:04.710Z] [metrics] africa candidates=12 picked=https://iafrica.com/ai-for-africas-development-initiative-wins-campaign-of-the-year-at-the-2026-prnews-platinum-awards/ score=7 domains=iafrica.com,techcabal.com,iafrica.com,techcabal.com,techcabal.com,techcabal.com,iafrica.com,techcabal.com
```
</details>
