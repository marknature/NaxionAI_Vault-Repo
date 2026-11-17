---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-55961e4f
created: 2026-10-25T06:00:24.228Z
jobId: 55961e4f-e27f-4296-94b4-b8c18e373f9b
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-25T06:00:21.767Z
finishedAt: 2026-10-25T06:00:24.228Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-10-25T06:00:21.767Z
- **Finished:** 2026-10-25T06:00:24.228Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (2.4s)
2. ✓ Dedupe + enrich — `pipeline` (2.5s)
3. ✓ Quality rank — `pipeline` (2.5s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-25T06:00:21.771Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-25T06:00:21.771Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-25T06:00:24.226Z] [history] 76 URLs posted in last 7d
[2026-10-25T06:00:24.227Z] No fresh Africa/AI news found today — skipping the post.
[2026-10-25T06:00:24.228Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
