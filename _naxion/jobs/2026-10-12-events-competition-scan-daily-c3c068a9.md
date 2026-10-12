---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-c3c068a9
created: 2026-10-12T05:50:04.952Z
jobId: c3c068a9-8b89-4263-800d-d10905f36d56
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-12T05:49:07.083Z
finishedAt: 2026-10-12T05:50:04.951Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-12T05:49:07.083Z
- **Finished:** 2026-10-12T05:50:04.951Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
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
1. ✓ Sweep event sources — `pipeline` (9.8s)
2. ✓ Dedupe + enrich — `pipeline` (10.0s)
3. ✓ Build events table — `pipeline` (57.6s)
4. ✓ Post to Telegram — `pipeline` (57.8s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-12

⭐ TOP PICK: TechCrunch Disrupt 2026 — High-visibility networking with the architects of next-gen tech | https://techcrunch.com/2026/10/11/48-hours-to-techcrunch-disrupt-2026-hear-directly-from-the-people-building-whats-next/

🎪 TechCrunch Disrupt 2026

1 free · 1 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-12T05:49:07.096Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-12T05:49:07.096Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-12T05:49:16.129Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-12T05:49:16.931Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-12T05:49:17.092Z] [history] 29 URLs posted in last 7d
[2026-10-12T05:49:17.094Z] [history] skip already-posted agentsforhumans.devpost.com
[2026-10-12T05:49:17.111Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-12T05:49:18.692Z] [enrich] techcrunch.com 103 → 1004 chars
[2026-10-12T05:49:18.810Z] [enrich] techcrunch.com 117 → 1018 chars
[2026-10-12T05:49:18.896Z] [enrich] theverge.com 95 → 996 chars
[2026-10-12T05:49:19.479Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-12T05:49:19.493Z] [enrich] techcrunch.com 83 → 984 chars
[2026-10-12T05:49:19.506Z] [enrich] theverge.com 95 → 996 chars
[2026-10-12T05:49:19.508Z] [enrich] theverge.com 92 → 993 chars
[2026-10-12T05:49:19.512Z] [enrich] theverge.com 73 → 974 chars
[2026-10-12T05:49:19.512Z] Formatting 20 event candidates into the scan table.
[2026-10-12T05:50:04.651Z] [tracker] 3 deadlines tracked
[2026-10-12T05:50:04.654Z] [metrics] events candidates=20 picked=https://techcrunch.com/2026/10/11/48-hours-to-techcrunch-disrupt-2026-hear-directly-from-the-people-building-whats-next/ score=? domains=techcrunch.com,techcrunch.com,theverge.com,theverge.com,theverge.com,theverge.com,techcrunch.com,theverge.com
[2026-10-12T05:50:04.951Z] Posted Events & Competition Scan to Telegram chat -1004307136262.
```
</details>
