---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-709210fa
created: 2026-11-15T05:33:52.149Z
jobId: 709210fa-e430-402e-a856-0989f9781f17
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-15T05:30:24.896Z
finishedAt: 2026-11-15T05:33:52.139Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-15T05:30:24.896Z
- **Finished:** 2026-11-15T05:33:52.139Z
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
1. ✓ Sweep event sources — `pipeline` (9.8s)
2. ✓ Dedupe + enrich — `pipeline` (9.9s)
3. ✓ Build events table — `pipeline` (206.5s)
4. ✓ Post to Telegram — `pipeline` (207.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-15

⭐ TOP PICK: TechZim Conference — A must-attend tech summit for innovation and entrepreneurship in Zimbabwe | https://www.techzimconference.com/

🚀 Coding Challenge: TechZim Hackathon

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-15T05:30:24.909Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-15T05:30:24.909Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-15T05:30:29.994Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-15T05:30:34.732Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-11-15T05:30:34.769Z] [history] 150 URLs posted in last 7d
[2026-11-15T05:30:34.921Z] [enrich] techcrunch.com 106 → 1007 chars
[2026-11-15T05:30:34.940Z] [enrich] techcrunch.com 114 → 1015 chars
[2026-11-15T05:30:34.942Z] [enrich] techcrunch.com 62 → 963 chars
[2026-11-15T05:30:34.956Z] [enrich] theverge.com 98 → 999 chars
[2026-11-15T05:30:34.964Z] [enrich] theverge.com 85 → 986 chars
[2026-11-15T05:30:36.111Z] [enrich] simonwillison.net 50 → 951 chars
[2026-11-15T05:30:40.060Z] [enrich] theverge.com 103 → 1004 chars
[2026-11-15T05:30:41.868Z] [enrich] arstechnica.com 95 → 996 chars
[2026-11-15T05:30:41.868Z] Formatting 20 event candidates into the scan table.
[2026-11-15T05:33:51.430Z] [tracker] 8 deadlines tracked
[2026-11-15T05:33:51.434Z] [metrics] events candidates=20 picked=https://www.techzimconference.com/ score=? domains=techcrunch.com,techcrunch.com,theverge.com,theverge.com,arstechnica.com,theverge.com,techcrunch.com,simonwillison.net
[2026-11-15T05:33:52.138Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
