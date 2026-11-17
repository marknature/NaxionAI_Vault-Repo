---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-049bd869
created: 2026-11-13T07:00:06.777Z
jobId: 049bd869-4c33-45af-b814-d9e87bf3c17c
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-13T07:00:03.422Z
finishedAt: 2026-11-13T07:00:06.777Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-13T07:00:03.422Z
- **Finished:** 2026-11-13T07:00:06.777Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (3.3s)
2. ✓ Dedupe + enrich — `pipeline` (3.3s)
3. ✓ Quality rank — `pipeline` (3.3s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-13T07:00:03.431Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-13T07:00:03.432Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-13T07:00:06.775Z] [history] 139 URLs posted in last 7d
[2026-11-13T07:00:06.776Z] No fresh World news found today — skipping the post.
[2026-11-13T07:00:06.777Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
