---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-54e0df2f
created: 2026-10-23T07:01:10.273Z
jobId: 54e0df2f-c0fd-4307-8ea5-1d577cf28f67
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-23T07:01:01.038Z
finishedAt: 2026-10-23T07:01:10.264Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-23T07:01:01.038Z
- **Finished:** 2026-10-23T07:01:10.264Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (8.8s)
2. ✓ Dedupe + enrich — `pipeline` (9.1s)
3. ✓ Quality rank — `pipeline` (9.1s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-23T07:01:01.186Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-23T07:01:01.186Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-23T07:01:10.241Z] [history] 67 URLs posted in last 7d
[2026-10-23T07:01:10.252Z] No fresh World news found today — skipping the post.
[2026-10-23T07:01:10.262Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
