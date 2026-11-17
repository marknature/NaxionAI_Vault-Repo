---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-04aa67af
created: 2026-10-21T07:10:49.496Z
jobId: 04aa67af-fa18-4dbd-b0b0-50e37c9da842
status: failed
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-21T06:00:29.130Z
finishedAt: 2026-10-21T07:10:49.495Z
---

# Africa AI news — BREAKING

- **Status:** failed
- **Template:** africa-ai-news
- **Started:** 2026-10-21T06:00:29.130Z
- **Finished:** 2026-10-21T07:10:49.495Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (6.7s)
2. ✓ Dedupe + enrich — `pipeline` (6.7s)
3. ✓ Quality rank — `pipeline` (189.4s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

## Error
```
This operation was aborted
```

<details><summary>Log</summary>

```
[2026-10-21T06:00:29.135Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-21T06:00:29.136Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-21T06:00:34.116Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-10-21T06:00:35.799Z] [africa] web search gathered 14 candidates (quality-filtered).
[2026-10-21T06:00:35.828Z] [history] 54 URLs posted in last 7d
[2026-10-21T06:00:35.829Z] [history] skip already-posted dlapiper.com
[2026-10-21T06:00:35.829Z] [history] skip already-posted ainowinstitute.org
[2026-10-21T06:00:35.829Z] [history] skip already-posted reuters.com
[2026-10-21T06:00:35.834Z] [filter] deduped 22 → 19 (spam/history removed)
[2026-10-21T06:00:36.533Z] [enrich] techcrunch.com 117 → 1018 chars
[2026-10-21T06:00:36.859Z] [enrich] techcabal.com 113 → 1014 chars
[2026-10-21T06:00:37.362Z] [enrich] techinafrica.com 127 → 1028 chars
[2026-10-21T06:00:38.695Z] [enrich] iafrica.com 138 → 1039 chars
[2026-10-21T06:00:38.740Z] [enrich] iafrica.com 102 → 1003 chars
[2026-10-21T06:00:41.931Z] [enrich] iafrica.com 111 → 1012 chars
[2026-10-21T06:03:38.579Z] [quality] scoring skipped: Unexpected non-whitespace character after JSON at position 146 (line 2 column 1) — keeping authority-sorted order
[2026-10-21T06:03:38.579Z] Picked 12 fresh candidates (top score 7) — drafting the daily card.
[2026-10-21T07:10:49.495Z] error: This operation was aborted
```
</details>
