---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-12f31eb5
created: 2026-10-22T07:02:34.573Z
jobId: 12f31eb5-8d66-4102-a6b7-60d3d11b0955
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-22T07:00:24.936Z
finishedAt: 2026-10-22T07:02:34.573Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-10-22T07:00:24.936Z
- **Finished:** 2026-10-22T07:02:34.573Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (129.6s)
2. ✓ Dedupe + enrich — `pipeline` (129.6s)
3. ✓ Quality rank — `pipeline` (129.6s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-22T07:00:24.940Z] Sweeping for today's World AI news (RSS + web search).
[2026-10-22T07:00:24.940Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-10-22T07:02:34.572Z] [history] 58 URLs posted in last 7d
[2026-10-22T07:02:34.572Z] No fresh World news found today — skipping the post.
[2026-10-22T07:02:34.573Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
