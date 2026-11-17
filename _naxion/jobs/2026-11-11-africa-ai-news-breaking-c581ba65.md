---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-c581ba65
created: 2026-11-11T06:00:58.921Z
jobId: c581ba65-3c98-463e-bb17-5bcbb5ba1dc8
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-11T06:00:47.729Z
finishedAt: 2026-11-11T06:00:58.920Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-11T06:00:47.729Z
- **Finished:** 2026-11-11T06:00:58.920Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (11.1s)
2. ✓ Dedupe + enrich — `pipeline` (11.2s)
3. ✓ Quality rank — `pipeline` (11.2s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-11T06:00:47.743Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-11T06:00:47.745Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-11T06:00:58.916Z] [history] 127 URLs posted in last 7d
[2026-11-11T06:00:58.917Z] No fresh Africa/AI news found today — skipping the post.
[2026-11-11T06:00:58.920Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
