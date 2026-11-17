---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-94a81e4f
created: 2026-10-16T07:14:29.618Z
jobId: 94a81e4f-8dc3-4081-9808-303ae9b4fddf
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-16T07:14:25.198Z
finishedAt: 2026-10-16T07:14:29.617Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-16T07:14:25.198Z
- **Finished:** 2026-10-16T07:14:29.617Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (4.0s)
2. ✓ Dedupe + enrich — `pipeline` (4.3s)
3. ✓ Quality rank — `pipeline` (4.3s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-16T07:14:25.247Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-16T07:14:25.247Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-16T07:14:29.596Z] [history] 32 URLs posted in last 7d
[2026-10-16T07:14:29.597Z] No fresh World news found today — skipping the post.
[2026-10-16T07:14:29.617Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
