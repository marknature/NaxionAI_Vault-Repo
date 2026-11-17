---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-e5878d90
created: 2026-11-17T07:05:09.102Z
jobId: e5878d90-dc83-4597-9027-45e2a69cfe00
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-17T07:04:37.748Z
finishedAt: 2026-11-17T07:05:09.089Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-17T07:04:37.748Z
- **Finished:** 2026-11-17T07:05:09.089Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (30.5s)
2. ✓ Dedupe + enrich — `pipeline` (30.8s)
3. ✓ Quality rank — `pipeline` (30.8s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-17T07:04:38.248Z] Started after 0s in the task queue.
[2026-11-17T07:04:38.248Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-17T07:04:38.249Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-17T07:05:09.062Z] [history] 159 URLs posted in last 7d
[2026-11-17T07:05:09.064Z] No fresh World news found today — skipping the post.
[2026-11-17T07:05:09.088Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
