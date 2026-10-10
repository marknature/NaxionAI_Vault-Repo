---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-92b24667
created: 2026-10-10T07:00:51.036Z
jobId: 92b24667-61d5-44c5-bca1-6fd01ac18801
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-10-10T07:00:25.448Z
finishedAt: 2026-10-10T07:00:51.035Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-10-10T07:00:25.448Z
- **Finished:** 2026-10-10T07:00:51.035Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (4.9s)
2. ✓ Dedupe + rank — `pipeline` (23.1s)
3. ✓ Build weekend card — `pipeline` (24.8s)
4. ✓ Post to Telegram — `pipeline` (25.6s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-10-10
Ukraine’s drones knock out AI data center belonging to "Russia’s Google"
Kick back and enjoy the break.

<details><summary>Log</summary>

```
[2026-10-10T07:00:25.451Z] Weekend sweep: Africa + World + SI queries in one pass.
[2026-10-10T07:00:29.555Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-10T07:00:30.391Z] [weekend] web search gathered 14 candidates (quality-filtered).
[2026-10-10T07:00:30.404Z] [history] 24 URLs posted in last 7d
[2026-10-10T07:00:30.404Z] [history] skip already-posted techcrunch.com
[2026-10-10T07:00:30.404Z] [history] skip already-posted reuters.com
[2026-10-10T07:00:30.409Z] [filter] deduped 22 → 20 (spam/history removed)
[2026-10-10T07:00:30.486Z] [enrich] simonwillison.net 56 → 957 chars
[2026-10-10T07:00:30.487Z] [enrich] techcrunch.com 103 → 1004 chars
[2026-10-10T07:00:30.519Z] [enrich] theverge.com 60 → 961 chars
[2026-10-10T07:00:40.930Z] [enrich] arstechnica.com 87 → 988 chars
[2026-10-10T07:00:42.047Z] [enrich] arstechnica.com 88 → 989 chars
[2026-10-10T07:00:42.056Z] [enrich] arstechnica.com 100 → 1001 chars
[2026-10-10T07:00:48.559Z] [quality] scored 12 candidates — top: #2:8 High impact/novelty regarding AI infrast | #1:7 High relevance (AI valuation), recent, t | #7:7 High relevance to cloud infrastructure/d
[2026-10-10T07:00:48.559Z] Picked 3 stories for the weekend card.
[2026-10-10T07:00:50.287Z] [metrics] weekend candidates=20 picked=https://arstechnica.com/gadgets/2026/10/ukraines-drones-knock-out-ai-data-center-belonging-to-russias-google/ score=8 domains=arstechnica.com,techcrunch.com,simonwillison.net,theverge.com,africanlawbusiness.com,facebook.com,youtube.com,facebook.com
[2026-10-10T07:00:51.035Z] Posted weekend digest to Telegram chat -1004307136262.
```
</details>
