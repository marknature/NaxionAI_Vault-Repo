---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-29665d28
created: 2026-10-26T07:25:57.784Z
jobId: 29665d28-9c42-4809-90c0-c8c3f682e677
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-26T07:25:19.292Z
finishedAt: 2026-10-26T07:25:57.752Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-26T07:25:19.292Z
- **Finished:** 2026-10-26T07:25:57.752Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (37.1s)
2. ✓ Dedupe + enrich — `pipeline` (38.2s)
3. ✓ Quality rank — `pipeline` (38.2s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-26T07:25:19.505Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-26T07:25:19.505Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-26T07:25:57.714Z] [history] 82 URLs posted in last 7d
[2026-10-26T07:25:57.717Z] No fresh World news found today — skipping the post.
[2026-10-26T07:25:57.752Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
