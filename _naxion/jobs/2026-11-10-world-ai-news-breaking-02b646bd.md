---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-02b646bd
created: 2026-11-10T07:00:27.443Z
jobId: 02b646bd-187d-48f2-878b-40d902d27a79
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-10T07:00:27.390Z
finishedAt: 2026-11-10T07:00:27.442Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-10T07:00:27.390Z
- **Finished:** 2026-11-10T07:00:27.442Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (0.0s)
2. ✓ Dedupe + enrich — `pipeline` (0.0s)
3. ✓ Quality rank — `pipeline` (0.0s)
4. · Build news card — `pipeline`
5. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-10T07:00:27.399Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-10T07:00:27.399Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-10T07:00:27.440Z] [history] 127 URLs posted in last 7d
[2026-11-10T07:00:27.441Z] No fresh World news found today — skipping the post.
[2026-11-10T07:00:27.442Z] [metrics] world candidates=0 picked=none score=? domains=
```
</details>
