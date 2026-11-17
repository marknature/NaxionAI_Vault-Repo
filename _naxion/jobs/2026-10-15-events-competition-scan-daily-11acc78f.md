---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-11acc78f
created: 2026-10-15T05:33:03.452Z
jobId: 11acc78f-38a2-4869-9d7b-78c43bd6b75f
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-15T05:30:29.302Z
finishedAt: 2026-10-15T05:33:03.452Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-15T05:30:29.302Z
- **Finished:** 2026-10-15T05:33:03.452Z
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
1. ✓ Sweep event sources — `pipeline` (29.3s)
2. ✓ Dedupe + enrich — `pipeline` (29.4s)
3. ✓ Build events table — `pipeline` (153.5s)
4. ✓ Post to Telegram — `pipeline` (154.1s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-15

⭐ TOP PICK: AMD Developer Hackathon: ACT II — why it is the one not to miss (TBA) | https://lablab.ai/ai-hackathons

🌍 AMD Developer Hackathon: ACT II

2 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-15T05:30:29.307Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-15T05:30:29.307Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-15T05:30:42.305Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-15T05:30:58.582Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-15T05:30:58.729Z] [history] 34 URLs posted in last 7d
[2026-10-15T05:30:59.125Z] [enrich] techcrunch.com 115 → 1016 chars
[2026-10-15T05:30:59.128Z] [enrich] techcrunch.com 116 → 1017 chars
[2026-10-15T05:30:59.130Z] [enrich] theverge.com 85 → 986 chars
[2026-10-15T05:30:59.136Z] [enrich] theverge.com 111 → 1012 chars
[2026-10-15T05:31:01.784Z] [enrich] theverge.com 90 → 991 chars
[2026-10-15T05:31:01.794Z] [enrich] theverge.com 85 → 986 chars
[2026-10-15T05:31:08.766Z] [enrich] techcrunch.com 123 → 1024 chars
[2026-10-15T05:31:09.582Z] [enrich] techcrunch.com 99 → 1000 chars
[2026-10-15T05:31:09.582Z] Formatting 20 event candidates into the scan table.
[2026-10-15T05:33:02.766Z] [tracker] 5 deadlines tracked
[2026-10-15T05:33:02.767Z] [metrics] events candidates=20 picked=https://lablab.ai/ai-hackathons score=? domains=techcrunch.com,techcrunch.com,techcrunch.com,theverge.com,techcrunch.com,theverge.com,theverge.com,theverge.com
[2026-10-15T05:33:03.451Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
