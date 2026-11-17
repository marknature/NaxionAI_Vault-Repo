---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-c156ca43
created: 2026-11-16T05:40:17.794Z
jobId: c156ca43-292d-451e-bbf7-a30d3dab41aa
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-16T05:30:08.296Z
finishedAt: 2026-11-16T05:40:17.793Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-16T05:30:08.296Z
- **Finished:** 2026-11-16T05:40:17.793Z
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
1. ✓ Sweep event sources — `pipeline` (8.2s)
2. ✓ Dedupe + enrich — `pipeline` (8.4s)
3. ✓ Build events table — `pipeline` (609.2s)
4. ✓ Post to Telegram — `pipeline` (609.4s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-16

⭐ TOP PICK: TBA — TBA | TBA

💻 Hackathon: Zimbabwe Tech Hackathon

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-16T05:30:08.359Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-16T05:30:08.361Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-16T05:30:14.426Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-16T05:30:16.560Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-11-16T05:30:16.790Z] [history] 155 URLs posted in last 7d
[2026-11-16T05:30:17.502Z] [enrich] arxiv.org 90 → 991 chars
[2026-11-16T05:30:17.711Z] [enrich] arxiv.org 71 → 972 chars
[2026-11-16T05:30:17.772Z] [enrich] arxiv.org 100 → 1001 chars
[2026-11-16T05:30:27.980Z] [enrich] arxiv.org 151 → 1052 chars
[2026-11-16T05:30:27.991Z] [enrich] arxiv.org 111 → 1012 chars
[2026-11-16T05:30:28.000Z] [enrich] arxiv.org 110 → 1011 chars
[2026-11-16T05:30:28.009Z] [enrich] arxiv.org 95 → 996 chars
[2026-11-16T05:30:28.010Z] [enrich] arxiv.org 140 → 1041 chars
[2026-11-16T05:30:28.010Z] Formatting 20 event candidates into the scan table.
[2026-11-16T05:40:17.530Z] [tracker] 9 deadlines tracked
[2026-11-16T05:40:17.532Z] [metrics] events candidates=20 picked=https://arxiv.org/abs/2611.17515 score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-16T05:40:17.793Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
