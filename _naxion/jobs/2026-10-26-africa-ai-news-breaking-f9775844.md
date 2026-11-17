---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-f9775844
created: 2026-10-26T11:33:58.424Z
jobId: f9775844-a939-487f-a457-30bdcf57275f
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-26T10:36:59.633Z
finishedAt: 2026-10-26T11:33:58.331Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-10-26T10:36:59.633Z
- **Finished:** 2026-10-26T11:33:58.331Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "chatId": "<existing>",
  "videoUrl": "<existing>"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (77.6s)
2. ✓ Dedupe + enrich — `pipeline` (77.6s)
3. ✓ Quality rank — `pipeline` (3417.9s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-26T10:36:59.851Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-26T10:36:59.851Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-26T10:38:17.449Z] [africa] web search gathered 18 candidates (quality-filtered).
[2026-10-26T10:38:17.456Z] [history] 82 URLs posted in last 7d
[2026-10-26T10:38:17.457Z] [history] skip already-posted facebook.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted reuters.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted ainowinstitute.org
[2026-10-26T10:38:17.457Z] [history] skip already-posted facebook.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted dlapiper.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted africatechsummit.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted africatechfestival.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted facebook.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted abmagazine.accaglobal.com
[2026-10-26T10:38:17.457Z] [history] skip already-posted counterpointresearch.com
[2026-10-26T10:38:17.457Z] [filter] deduped 18 → 8 (spam/history removed)
[2026-10-26T10:38:40.661Z] [enrich] facebook.com 147 → 1048 chars
[2026-10-26T10:38:41.558Z] [enrich] linkedin.com 144 → 332 chars
[2026-10-26T11:33:57.781Z] [quality] scoring skipped: This operation was aborted — keeping authority-sorted order
[2026-10-26T11:33:57.781Z] [gate] top score 7 < threshold 8 — not breaking enough — queuing as draft, not posting to Telegram
[2026-10-26T11:33:58.330Z] [metrics] africa candidates=8 picked=https://iafrica.com/zimbabwe-opens-ai-for-impact-challenge-with-up-to-80000-in-funding/ score=7 domains=iafrica.com,qz.com,vivatech.com,facebook.com,linkedin.com,mctafrica.org,africatechsummit.com,globalafricatech.com
```
</details>
