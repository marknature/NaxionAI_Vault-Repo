---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-6144bb5a
created: 2026-11-19T05:36:31.166Z
jobId: 6144bb5a-2a33-4dcc-b7b3-712c8492181c
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-19T05:30:24.540Z
finishedAt: 2026-11-19T05:36:31.154Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-19T05:30:24.540Z
- **Finished:** 2026-11-19T05:36:31.154Z
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
1. ✓ Sweep event sources — `pipeline` (44.7s)
2. ✓ Dedupe + enrich — `pipeline` (44.7s)
3. ✓ Build events table — `pipeline` (365.8s)
4. ✓ Post to Telegram — `pipeline` (366.6s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-19

⭐ TOP PICK: Zimbabwe Tech Summit 2026 — Unlocking Zimbabwe’s Tech Potential with Global Experts | https://www.zimtechsummit.com

💻 Zimbabwe Tech Hackathon 2026

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-19T05:30:24.551Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-19T05:30:24.551Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-19T05:30:29.517Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-19T05:31:09.206Z] [events] web search gathered 10 candidates (quality-filtered).
[2026-11-19T05:31:09.258Z] [history] 165 URLs posted in last 7d
[2026-11-19T05:31:09.449Z] [enrich] arxiv.org 126 → 1027 chars
[2026-11-19T05:31:09.710Z] [enrich] arxiv.org 71 → 972 chars
[2026-11-19T05:31:09.714Z] [enrich] arxiv.org 72 → 973 chars
[2026-11-19T05:31:10.399Z] [enrich] arxiv.org 158 → 1059 chars
[2026-11-19T05:31:10.399Z] [enrich] arxiv.org 101 → 1002 chars
[2026-11-19T05:31:10.409Z] [enrich] arxiv.org 110 → 1011 chars
[2026-11-19T05:31:10.413Z] [enrich] arxiv.org 102 → 1003 chars
[2026-11-19T05:31:10.640Z] [enrich] arxiv.org 95 → 996 chars
[2026-11-19T05:31:10.640Z] Formatting 18 event candidates into the scan table.
[2026-11-19T05:36:30.333Z] [tracker] 10 deadlines tracked
[2026-11-19T05:36:30.334Z] [metrics] events candidates=18 picked=https://www.zimtechsummit.com score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-19T05:36:31.154Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
