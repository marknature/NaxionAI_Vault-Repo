---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-429155b0
created: 2026-11-17T05:35:12.268Z
jobId: 429155b0-9d66-49ec-a9a0-952e7a479cdb
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-17T05:30:23.567Z
finishedAt: 2026-11-17T05:35:12.268Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-17T05:30:23.567Z
- **Finished:** 2026-11-17T05:35:12.268Z
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
1. ✓ Sweep event sources — `pipeline` (6.5s)
2. ✓ Dedupe + enrich — `pipeline` (6.7s)
3. ✓ Build events table — `pipeline` (288.4s)
4. ✓ Post to Telegram — `pipeline` (288.7s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-17

⭐ TOP PICK: Dreamteam Raises $53M to Build an AI-Native CRM Platform — Dreamteam Raises $53M to Build an AI-Native CRM Platform | URL

**💻 hackathon/coding challenge**

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-17T05:30:23.578Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-17T05:30:23.578Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-17T05:30:27.904Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-17T05:30:30.067Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-11-17T05:30:30.261Z] [history] 158 URLs posted in last 7d
[2026-11-17T05:30:30.266Z] [filter] deduped 22 → 21 (spam/history removed)
[2026-11-17T05:30:30.390Z] [enrich] theverge.com 70 → 971 chars
[2026-11-17T05:30:30.394Z] [enrich] theverge.com 99 → 1000 chars
[2026-11-17T05:30:30.395Z] [enrich] techcrunch.com 99 → 1000 chars
[2026-11-17T05:30:30.621Z] [enrich] ventureburn.com 101 → 789 chars
[2026-11-17T05:30:30.662Z] [enrich] ventureburn.com 103 → 780 chars
[2026-11-17T05:30:30.695Z] [enrich] ventureburn.com 88 → 700 chars
[2026-11-17T05:30:30.716Z] [enrich] ventureburn.com 83 → 819 chars
[2026-11-17T05:30:39.003Z] [enrich] farmnport.com 143 → 482 chars
[2026-11-17T05:30:39.004Z] Formatting 20 event candidates into the scan table.
[2026-11-17T05:35:11.982Z] [tracker] no machine-readable deadlines this run
[2026-11-17T05:35:12.026Z] [metrics] events candidates=20 picked=https://ventureburn.com/stark-future-raises-150m-electric-motorcycles/ score=? domains=ventureburn.com,ventureburn.com,techcrunch.com,theverge.com,ventureburn.com,ventureburn.com,theverge.com,farmnport.com
[2026-11-17T05:35:12.267Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
