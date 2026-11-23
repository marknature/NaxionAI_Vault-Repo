---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-5a36f6b2
created: 2026-11-23T17:40:43.716Z
jobId: 5a36f6b2-f838-4e64-b7af-e5d389d7dd79
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-11-23T17:38:29.222Z
finishedAt: 2026-11-23T17:40:43.715Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-11-23T17:38:29.222Z
- **Finished:** 2026-11-23T17:40:43.715Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (7.2s)
2. ✓ Dedupe + rank — `pipeline` (66.3s)
3. ✓ Build weekend card — `pipeline` (133.7s)
4. ✓ Post to Telegram — `pipeline` (134.5s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-11-23
Title
Enjoy your weekend, here’s hoping you find some time for fun and innovation!

<details><summary>Log</summary>

```
[2026-11-23T17:38:29.236Z] Weekend sweep: Africa + World queries in one pass.
[2026-11-23T17:38:34.667Z] [weekend] web search gathered 14 candidates (quality-filtered).
[2026-11-23T17:38:36.416Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-23T17:38:36.477Z] [history] 181 URLs posted in last 7d
[2026-11-23T17:38:36.479Z] [history] skip already-posted continenten.com
[2026-11-23T17:38:36.479Z] [history] skip already-posted openai.com
[2026-11-23T17:38:36.479Z] [history] skip already-posted deepai.org
[2026-11-23T17:38:36.483Z] [filter] deduped 22 → 19 (spam/history removed)
[2026-11-23T17:38:36.902Z] [enrich] techcrunch.com 122 → 1023 chars
[2026-11-23T17:38:37.767Z] [enrich] blog.google 81 → 982 chars
[2026-11-23T17:38:42.926Z] [enrich] deepmind.google 105 → 1006 chars
[2026-11-23T17:38:43.157Z] [enrich] huggingface.co 94 → 995 chars
[2026-11-23T17:38:45.100Z] [enrich] blogs.nvidia.com 108 → 1009 chars
[2026-11-23T17:38:45.111Z] [enrich] techcabal.com 99 → 1000 chars
[2026-11-23T17:39:35.500Z] [quality] scored 1 candidates — top: #1:8 high relevance globally, recent, from ti | #2:7  | #3:7 
[2026-11-23T17:39:35.500Z] Picked 3 stories for the weekend card.
[2026-11-23T17:40:42.972Z] [metrics] weekend candidates=19 picked=https://techcrunch.com/2026/11/23/amazon-snaps-up-decarts-ai-optimization-tech-for-7-5b-as-it-prepares-to-sell-trainium-chips/ score=8 domains=techcrunch.com,blogs.nvidia.com,deepmind.google,techcabal.com,huggingface.co,blog.google,theverge.com,techcrunch.com
[2026-11-23T17:40:43.715Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
