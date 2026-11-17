---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-1c2e8215
created: 2026-11-16T07:00:26.995Z
jobId: 1c2e8215-63b3-4ae8-9cac-4cc4baabbf29
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-16T07:00:20.525Z
finishedAt: 2026-11-16T07:00:26.994Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-16T07:00:20.525Z
- **Finished:** 2026-11-16T07:00:26.994Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (6.4s)
2. ✓ Dedupe + enrich — `pipeline` (6.4s)
3. ✓ Quality rank — `pipeline` (6.4s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-16T07:00:20.558Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-16T07:00:20.559Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-16T07:00:26.991Z] [history] 157 URLs posted in last 7d
[2026-11-16T07:00:26.992Z] No fresh World news found today — skipping the post.
[2026-11-16T07:00:26.994Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
