---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-f3471da1
created: 2026-10-15T07:03:15.538Z
jobId: f3471da1-304d-43f5-a416-afd49ae286b5
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-15T07:02:13.775Z
finishedAt: 2026-10-15T07:03:15.538Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-15T07:02:13.775Z
- **Finished:** 2026-10-15T07:03:15.538Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (61.6s)
2. ✓ Dedupe + enrich — `pipeline` (61.7s)
3. ✓ Quality rank — `pipeline` (61.7s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-15T07:02:13.836Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-15T07:02:13.836Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-15T07:03:15.522Z] [history] 31 URLs posted in last 7d
[2026-10-15T07:03:15.525Z] No fresh World news found today — skipping the post.
[2026-10-15T07:03:15.537Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
