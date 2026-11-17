---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-af828354
created: 2026-10-29T07:48:54.096Z
jobId: af828354-696f-4cc4-85a6-2363ef2189f2
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-29T07:48:53.787Z
finishedAt: 2026-10-29T07:48:54.095Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-29T07:48:53.787Z
- **Finished:** 2026-10-29T07:48:54.095Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (0.1s)
2. ✓ Dedupe + enrich — `pipeline` (0.2s)
3. ✓ Quality rank — `pipeline` (0.3s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-29T07:48:53.844Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-29T07:48:53.844Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-29T07:48:54.075Z] [history] 101 URLs posted in last 7d
[2026-10-29T07:48:54.094Z] No fresh World news found today — skipping the post.
[2026-10-29T07:48:54.095Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
