---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-7f89dd92
created: 2026-11-10T08:00:13.296Z
jobId: 7f89dd92-1c00-4151-9ab1-5e24ad88f67f
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-10T08:00:13.153Z
finishedAt: 2026-11-10T08:00:13.294Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-10T08:00:13.153Z
- **Finished:** 2026-11-10T08:00:13.294Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "chatId": "<existing>",
  "videoUrl": "<existing>"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (0.0s)
2. ✓ Dedupe + enrich — `pipeline` (0.1s)
3. ✓ Quality rank — `pipeline` (0.1s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-10T08:00:13.181Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-10T08:00:13.182Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-10T08:00:13.285Z] [history] 127 URLs posted in last 7d
[2026-11-10T08:00:13.290Z] No fresh Africa/AI news found today — skipping the post.
[2026-11-10T08:00:13.293Z] [metrics] africa candidates=0 picked=none score=? domains=
```
</details>
