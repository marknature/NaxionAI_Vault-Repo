---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-2584fad1
created: 2026-10-16T05:39:47.703Z
jobId: 2584fad1-f2d9-40f3-b8fa-37ff8e1a089d
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-16T05:36:38.505Z
finishedAt: 2026-10-16T05:39:47.701Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-16T05:36:38.505Z
- **Finished:** 2026-10-16T05:39:47.701Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406",
  "ratio": "80% free, 20% paid",
  "regions": [
    "Zimbabwe",
    "South Africa",
    "Africa"
  ],
  "categories": [
    "summits",
    "conferences",
    "hackathons",
    "innovation challenges",
    "expos",
    "startup pitch",
    "corporate software competitions"
  ]
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (12.4s)
2. ✓ Dedupe + enrich — `pipeline` (12.5s)
3. ✓ Build events table — `pipeline` (188.1s)
4. ✓ Post to Telegram — `pipeline` (189.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-16

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-16T05:36:38.526Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-16T05:36:38.527Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-16T05:36:50.946Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-16T05:36:50.954Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-16T05:36:50.991Z] [history] 29 URLs posted in last 7d
[2026-10-16T05:36:50.992Z] [history] skip already-posted lablab.ai
[2026-10-16T05:36:51.006Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-16T05:36:51.173Z] [enrich] theverge.com 80 → 981 chars
[2026-10-16T05:36:51.180Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-16T05:36:51.200Z] [enrich] techcrunch.com 111 → 1012 chars
[2026-10-16T05:36:51.264Z] [enrich] theverge.com 65 → 966 chars
[2026-10-16T05:36:51.403Z] [enrich] ventureburn.com 86 → 790 chars
[2026-10-16T05:36:51.415Z] [enrich] ventureburn.com 85 → 802 chars
[2026-10-16T05:36:51.602Z] [enrich] ventureburn.com 75 → 810 chars
[2026-10-16T05:36:51.667Z] [enrich] ventureburn.com 82 → 804 chars
[2026-10-16T05:36:51.667Z] Formatting 20 event candidates into the scan table.
[2026-10-16T05:39:46.601Z] [tracker] no machine-readable deadlines this run
[2026-10-16T05:39:46.674Z] [metrics] events candidates=20 picked=https://techcrunch.com/2026/10/15/when-it-came-to-cal-ais-viral-success-a-small-army-of-influencers-paid-off/ score=? domains=techcrunch.com,theverge.com,ventureburn.com,ventureburn.com,ventureburn.com,theverge.com,ventureburn.com,theverge.com
[2026-10-16T05:39:47.700Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
