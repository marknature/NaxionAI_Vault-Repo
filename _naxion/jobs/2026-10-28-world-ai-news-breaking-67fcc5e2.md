---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-67fcc5e2
created: 2026-10-28T07:18:24.808Z
jobId: 67fcc5e2-a017-469f-b541-63e89aaf5d4a
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-28T07:17:35.966Z
finishedAt: 2026-10-28T07:18:24.445Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-28T07:17:35.966Z
- **Finished:** 2026-10-28T07:18:24.445Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (8.7s)
2. ✓ Dedupe + enrich — `pipeline` (41.9s)
3. ✓ Quality rank — `pipeline` (41.9s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-28T07:17:39.420Z] Started after 3s in the task queue.
[2026-10-28T07:17:39.835Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-28T07:17:39.918Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-28T07:18:21.663Z] [history] 91 URLs posted in last 7d
[2026-10-28T07:18:21.689Z] No fresh World news found today — skipping the post.
[2026-10-28T07:18:24.040Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
