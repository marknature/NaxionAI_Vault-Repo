---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-a7d43a14
created: 2026-11-16T06:53:07.542Z
jobId: a7d43a14-da04-41ce-b651-74c16f2db877
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-16T06:52:54.108Z
finishedAt: 2026-11-16T06:53:07.541Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-16T06:52:54.108Z
- **Finished:** 2026-11-16T06:53:07.541Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (13.3s)
2. ✓ Dedupe + enrich — `pipeline` (13.4s)
3. ✓ Quality rank — `pipeline` (13.4s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-16T06:52:54.118Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-16T06:52:54.118Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-16T06:53:07.532Z] [history] 157 URLs posted in last 7d
[2026-11-16T06:53:07.535Z] No fresh Africa/AI news found today — skipping the post.
[2026-11-16T06:53:07.540Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
