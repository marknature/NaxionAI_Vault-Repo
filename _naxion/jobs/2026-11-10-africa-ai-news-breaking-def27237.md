---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-def27237
created: 2026-11-10T06:35:23.448Z
jobId: def27237-8dc9-4eb9-ba15-54cace596752
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-10T06:35:22.599Z
finishedAt: 2026-11-10T06:35:23.406Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-10T06:35:22.599Z
- **Finished:** 2026-11-10T06:35:23.406Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (0.0s)
2. ✓ Dedupe + enrich — `pipeline` (0.8s)
3. ✓ Quality rank — `pipeline` (0.8s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-10T06:35:22.610Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-10T06:35:22.611Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-10T06:35:23.404Z] [history] 127 URLs posted in last 7d
[2026-11-10T06:35:23.405Z] No fresh Africa/AI news found today — skipping the post.
[2026-11-10T06:35:23.406Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
