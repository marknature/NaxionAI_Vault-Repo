---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-948c3005
created: 2026-10-22T06:58:59.013Z
jobId: 948c3005-a501-477a-ad86-224a7db9c47c
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-22T06:52:58.453Z
finishedAt: 2026-10-22T06:58:59.013Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-10-22T06:52:58.453Z
- **Finished:** 2026-10-22T06:58:59.013Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (360.5s)
2. ✓ Dedupe + enrich — `pipeline` (360.6s)
3. ✓ Quality rank — `pipeline` (360.6s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-22T06:52:58.459Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-10-22T06:52:58.460Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-10-22T06:58:59.011Z] [history] 58 URLs posted in last 7d
[2026-10-22T06:58:59.012Z] No fresh Africa/AI news found today — skipping the post.
[2026-10-22T06:58:59.013Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
