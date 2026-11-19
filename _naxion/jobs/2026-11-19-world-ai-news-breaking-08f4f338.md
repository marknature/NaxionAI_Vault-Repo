---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-08f4f338
created: 2026-11-19T07:17:29.650Z
jobId: 08f4f338-1e28-4607-b061-bcf224fdaaec
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-19T07:17:20.558Z
finishedAt: 2026-11-19T07:17:29.650Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-19T07:17:20.558Z
- **Finished:** 2026-11-19T07:17:29.650Z
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
2. ✓ Dedupe + enrich — `pipeline` (8.8s)
3. ✓ Quality rank — `pipeline` (8.8s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-19T07:17:20.869Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-19T07:17:20.870Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-19T07:17:29.649Z] [history] 167 URLs posted in last 7d
[2026-11-19T07:17:29.649Z] No fresh World news found today — skipping the post.
[2026-11-19T07:17:29.650Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
