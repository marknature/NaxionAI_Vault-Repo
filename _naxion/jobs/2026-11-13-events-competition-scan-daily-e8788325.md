---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-e8788325
created: 2026-11-13T05:34:24.683Z
jobId: e8788325-e589-4bbe-963b-23580ee02e61
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-13T05:30:08.659Z
finishedAt: 2026-11-13T05:34:24.682Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-13T05:30:08.659Z
- **Finished:** 2026-11-13T05:34:24.682Z
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
1. ✓ Sweep event sources — `pipeline` (6.9s)
2. ✓ Dedupe + enrich — `pipeline` (7.1s)
3. ✓ Build events table — `pipeline` (255.2s)
4. ✓ Post to Telegram — `pipeline` (256.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-13

⭐ TOP PICK: TBA — TBA | TBA

💡 Why attend: Gain insights and connect with industry leaders on the latest tech trends and innovations.

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-13T05:30:08.669Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-13T05:30:08.669Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-13T05:30:15.091Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-13T05:30:15.581Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-13T05:30:15.768Z] [history] 137 URLs posted in last 7d
[2026-11-13T05:30:15.983Z] [enrich] theverge.com 93 → 994 chars
[2026-11-13T05:30:15.985Z] [enrich] theverge.com 103 → 1004 chars
[2026-11-13T05:30:15.986Z] [enrich] theverge.com 100 → 1001 chars
[2026-11-13T05:30:15.987Z] [enrich] theverge.com 73 → 974 chars
[2026-11-13T05:30:20.931Z] [enrich] microsoft.com 133 → 1034 chars
[2026-11-13T05:30:21.828Z] [enrich] support.microsoft.com 135 → 1036 chars
[2026-11-13T05:30:21.860Z] [enrich] support.microsoft.com 134 → 1035 chars
[2026-11-13T05:30:25.527Z] [enrich] arstechnica.com 104 → 251 chars
[2026-11-13T05:30:25.527Z] Formatting 20 event candidates into the scan table.
[2026-11-13T05:34:23.874Z] [tracker] 7 deadlines tracked
[2026-11-13T05:34:23.885Z] [metrics] events candidates=20 picked=https://support.microsoft.com/en-us/windows/how-to-get-help-in-windows-711b6492-0435-0038-8706-7c6b0feb200a score=? domains=support.microsoft.com,support.microsoft.com,microsoft.com,arstechnica.com,theverge.com,theverge.com,theverge.com,theverge.com
[2026-11-13T05:34:24.682Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
