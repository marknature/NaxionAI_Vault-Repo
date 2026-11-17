---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-6b9c7b5d
created: 2026-10-14T07:02:21.092Z
jobId: 6b9c7b5d-d206-4795-a206-3fa7b2609931
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-14T07:01:14.316Z
finishedAt: 2026-10-14T07:02:21.091Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-14T07:01:14.316Z
- **Finished:** 2026-10-14T07:02:21.091Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (66.8s)
2. ✓ Dedupe + enrich — `pipeline` (66.8s)
3. ✓ Quality rank — `pipeline` (66.8s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-14T07:01:14.321Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-14T07:01:14.322Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-14T07:02:21.090Z] [history] 34 URLs posted in last 7d
[2026-10-14T07:02:21.091Z] No fresh World news found today — skipping the post.
[2026-10-14T07:02:21.091Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
