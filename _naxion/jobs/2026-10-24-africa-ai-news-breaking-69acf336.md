---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-69acf336
created: 2026-10-24T10:03:19.826Z
jobId: 69acf336-0920-401a-b180-6ac60c98f6af
status: failed
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-24T06:00:27.312Z
finishedAt: 2026-10-24T10:03:19.826Z
---

# Africa AI news — BREAKING

- **Status:** failed
- **Template:** africa-ai-news
- **Started:** 2026-10-24T06:00:27.312Z
- **Finished:** 2026-10-24T10:03:19.826Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (6.4s)
2. ✓ Dedupe + enrich — `pipeline` (6.4s)
3. ✓ Quality rank — `pipeline` (7377.4s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

## Error
```
This operation was aborted
```

<details><summary>Log</summary>

```
[2026-10-24T06:00:27.316Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-24T06:00:27.316Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-24T06:00:33.581Z] [africa] web search gathered 18 candidates (quality-filtered).
[2026-10-24T06:00:33.697Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-10-24T06:00:33.715Z] [history] 71 URLs posted in last 7d
[2026-10-24T06:00:33.716Z] [history] skip already-posted techinafrica.com
[2026-10-24T06:00:33.716Z] [history] skip already-posted daily.dev
[2026-10-24T06:00:33.716Z] [history] skip already-posted daily.dev
[2026-10-24T06:00:33.716Z] [history] skip already-posted reuters.com
[2026-10-24T06:00:33.716Z] [history] skip already-posted ainowinstitute.org
[2026-10-24T06:00:33.716Z] [history] skip already-posted facebook.com
[2026-10-24T06:00:33.716Z] [history] skip already-posted dlapiper.com
[2026-10-24T06:00:33.716Z] [history] skip already-posted africatechsummit.com
[2026-10-24T06:00:33.716Z] [history] skip already-posted africatechfestival.com
[2026-10-24T06:00:33.717Z] [filter] deduped 26 → 17 (spam/history removed)
[2026-10-24T06:00:34.301Z] [enrich] techinafrica.com 104 → 569 chars
[2026-10-24T06:00:34.949Z] [enrich] arstechnica.com 114 → 1015 chars
[2026-10-24T06:00:36.144Z] [enrich] iafrica.com 97 → 998 chars
[2026-10-24T06:00:43.469Z] [enrich] daily.dev 204 → 359 chars
[2026-10-24T08:03:24.655Z] [quality] scoring skipped: This operation was aborted — keeping authority-sorted order
[2026-10-24T08:03:24.740Z] Picked 12 fresh candidates (top score 7) — drafting the daily card.
[2026-10-24T10:03:19.826Z] error: This operation was aborted
```
</details>
