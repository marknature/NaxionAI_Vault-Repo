---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-aa934824
created: 2026-11-23T05:39:54.294Z
jobId: aa934824-2a0f-464c-96e6-552c94cb819a
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-23T05:30:08.992Z
finishedAt: 2026-11-23T05:39:54.294Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-23T05:30:08.992Z
- **Finished:** 2026-11-23T05:39:54.294Z
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
1. ✓ Sweep event sources — `pipeline` (38.0s)
2. ✓ Dedupe + enrich — `pipeline` (38.2s)
3. ✓ Build events table — `pipeline` (574.6s)
4. ✓ Post to Telegram — `pipeline` (585.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-23

⭐ TOP PICK: Global AI Hackathon - 2026-11-23 | https://www.devpost.com/hackathons/global-ai-hackathon

💻 Global AI Hackathon

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-23T05:30:09.000Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-23T05:30:09.000Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-23T05:30:21.704Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-23T05:30:47.015Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-23T05:30:47.228Z] [history] 177 URLs posted in last 7d
[2026-11-23T05:30:47.228Z] [history] skip already-posted support.microsoft.com
[2026-11-23T05:30:47.232Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-11-23T05:30:48.723Z] [enrich] techcrunch.com 97 → 998 chars
[2026-11-23T05:30:49.142Z] [enrich] techcrunch.com 110 → 1011 chars
[2026-11-23T05:30:49.607Z] [enrich] theverge.com 89 → 990 chars
[2026-11-23T05:30:49.610Z] [enrich] theverge.com 93 → 994 chars
[2026-11-23T05:30:49.837Z] [enrich] theverge.com 89 → 990 chars
[2026-11-23T05:30:50.546Z] [enrich] theverge.com 105 → 1006 chars
[2026-11-23T05:30:59.991Z] [enrich] support.microsoft.com 130 → 424 chars
[2026-11-23T05:31:00.039Z] [enrich] support.microsoft.com 149 → 239 chars
[2026-11-23T05:31:00.039Z] Formatting 20 event candidates into the scan table.
[2026-11-23T05:39:43.590Z] [tracker] 9 deadlines tracked
[2026-11-23T05:39:43.593Z] [metrics] events candidates=20 picked=https://www.devpost.com/hackathons/global-ai-hackathon score=? domains=support.microsoft.com,support.microsoft.com,techcrunch.com,theverge.com,techcrunch.com,theverge.com,theverge.com,theverge.com
[2026-11-23T05:39:54.293Z] Telegram post failed: telegram send failed: fetch failed
```
</details>
