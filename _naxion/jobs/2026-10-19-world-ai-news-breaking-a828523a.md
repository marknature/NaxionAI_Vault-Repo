---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-a828523a
created: 2026-10-19T07:09:31.920Z
jobId: a828523a-087f-4d6d-b2d5-16d72dd36d0c
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-19T07:09:30.197Z
finishedAt: 2026-10-19T07:09:31.920Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-19T07:09:30.197Z
- **Finished:** 2026-10-19T07:09:31.920Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (1.7s)
2. ✓ Dedupe + enrich — `pipeline` (1.7s)
3. ✓ Quality rank — `pipeline` (1.7s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-19T07:09:30.204Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-19T07:09:30.204Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-19T07:09:31.918Z] [history] 49 URLs posted in last 7d
[2026-10-19T07:09:31.919Z] No fresh World news found today — skipping the post.
[2026-10-19T07:09:31.920Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
