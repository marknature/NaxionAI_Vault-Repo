---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-4b241b4a
created: 2026-11-08T07:00:26.267Z
jobId: 4b241b4a-2163-46b3-b1e0-b8945cdca729
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-11-08T07:00:06.456Z
finishedAt: 2026-11-08T07:00:26.267Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-11-08T07:00:06.456Z
- **Finished:** 2026-11-08T07:00:26.267Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (7.9s)
2. ✓ Dedupe + rank — `pipeline` (17.6s)
3. ✓ Build weekend card — `pipeline` (19.5s)
4. ✓ Post to Telegram — `pipeline` (19.8s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-11-08
Megaspeed exec was recruited to spy on Nvidia CEO, according to US intelligence memo
Enjoy the break and stay unplugged.

<details><summary>Log</summary>

```
[2026-11-08T07:00:06.475Z] Weekend sweep: Africa + World queries in one pass.
[2026-11-08T07:00:12.480Z] [weekend] web search gathered 16 candidates (quality-filtered).
[2026-11-08T07:00:14.339Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-08T07:00:14.361Z] [history] 120 URLs posted in last 7d
[2026-11-08T07:00:14.362Z] [history] skip already-posted daily.dev
[2026-11-08T07:00:14.362Z] [history] skip already-posted daily.dev
[2026-11-08T07:00:14.362Z] [history] skip already-posted daily.dev
[2026-11-08T07:00:14.362Z] [history] skip already-posted daily.dev
[2026-11-08T07:00:14.362Z] [history] skip already-posted whitehouse.gov
[2026-11-08T07:00:14.362Z] [history] skip already-posted nextgov.com
[2026-11-08T07:00:14.363Z] [history] skip already-posted blog.intimetec.com
[2026-11-08T07:00:14.378Z] [filter] deduped 24 → 17 (spam/history removed)
[2026-11-08T07:00:14.390Z] [enrich] techcrunch.com 113 → 1014 chars
[2026-11-08T07:00:14.402Z] [enrich] theverge.com 115 → 1016 chars
[2026-11-08T07:00:14.402Z] [enrich] simonwillison.net 112 → 1013 chars
[2026-11-08T07:00:14.510Z] [enrich] techcrunch.com 104 → 1005 chars
[2026-11-08T07:00:16.639Z] [enrich] iafrica.com 113 → 1014 chars
[2026-11-08T07:00:24.077Z] [quality] scored 12 candidates — top: #2:8 High-impact geopolitical/corporate espio | #6:7 High-relevance analysis of infrastructur | #9:6 Significant policy shift in government t
[2026-11-08T07:00:24.077Z] Picked 3 stories for the weekend card.
[2026-11-08T07:00:26.001Z] [metrics] weekend candidates=17 picked=https://techcrunch.com/2026/11/07/chinese-exec-was-recruited-to-spy-on-nvidia-ceo-according-to-us-intelligence-memo/ score=8 domains=techcrunch.com,techcrunch.com,govciomedia.com,iafrica.com,iafrica.com,youtube.com,reddit.com,coingeek.com
[2026-11-08T07:00:26.267Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
