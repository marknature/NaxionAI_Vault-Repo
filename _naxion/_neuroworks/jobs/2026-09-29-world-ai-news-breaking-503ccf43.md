---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-503ccf43
created: 2026-09-29T13:16:02.717Z
jobId: 503ccf43-4762-43c8-a6de-0e80ae44846c
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-09-29T12:54:46.417Z
finishedAt: 2026-09-29T13:16:02.716Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-09-29T12:54:46.417Z
- **Finished:** 2026-09-29T13:16:02.716Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "chatId": "-1004307136262"
}
```

<details><summary>Log</summary>

```
[2026-09-29T12:54:46.432Z] Sweeping for today's World AI news (RSS + web search).
[2026-09-29T12:54:46.432Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-09-29T13:12:10.022Z] [world] web search gathered 16 candidates (quality-filtered).
[2026-09-29T13:12:10.037Z] [history] 28 URLs posted in last 7d
[2026-09-29T13:12:10.037Z] [history] skip already-posted openai.com
[2026-09-29T13:12:10.040Z] [filter] deduped 16 → 15 (spam/history removed)
[2026-09-29T13:12:12.220Z] [enrich] chatgpt.com 130 → 549 chars
[2026-09-29T13:12:12.542Z] [enrich] ai.google 124 → 1025 chars
[2026-09-29T13:12:12.800Z] [enrich] support.google.com 153 → 1054 chars
[2026-09-29T13:12:13.274Z] [enrich] support.google.com 145 → 1046 chars
[2026-09-29T13:16:02.707Z] [quality] scored 12 candidates — top: #4:6 Relevant to AI/Tech, recent, and credibl | #10:5 Recent and relevant to AI/Tech, but low  | #13:5 
[2026-09-29T13:16:02.708Z] [gate] top score 6 < threshold 8 — not breaking enough — queuing as draft, not posting to Telegram
[2026-09-29T13:16:02.715Z] [metrics] world candidates=12 picked=https://stackoverflow.com/questions/34967847/generate-access-token-instagram-api-without-having-to-log-in score=6 domains=stackoverflow.com,stackoverflow.com,zhihu.com,zhihu.com,zhihu.com,agents.meta.stackoverflow.com,chatgpt.com,ai.google
```
</details>
