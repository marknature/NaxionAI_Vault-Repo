---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-c007df15
created: 2026-11-04T05:30:29.761Z
jobId: c007df15-ac75-4032-94a2-3a04c4bf29eb
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-04T05:30:15.199Z
finishedAt: 2026-11-04T05:30:29.760Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-04T05:30:15.199Z
- **Finished:** 2026-11-04T05:30:29.760Z
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
1. ✓ Sweep event sources — `pipeline` (9.3s)
2. ✓ Dedupe + enrich — `pipeline` (9.3s)
3. ✓ Build events table — `pipeline` (13.8s)
4. ✓ Post to Telegram — `pipeline` (14.6s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-04

⭐ TOP PICK: #BuildHybridAI 2026 — $30,000 prize pool for hybrid cloud/on-device AI apps | https://firebasehybridaihackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 #BuildHybridAI 2026

2 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-04T05:30:15.205Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-04T05:30:15.205Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-04T05:30:20.510Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-04T05:30:24.529Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-11-04T05:30:24.551Z] [history] 111 URLs posted in last 7d
[2026-11-04T05:30:24.551Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-04T05:30:24.554Z] [filter] deduped 22 → 21 (spam/history removed)
[2026-11-04T05:30:25.149Z] [enrich] arxiv.org 103 → 1004 chars
[2026-11-04T05:30:25.182Z] [enrich] arxiv.org 128 → 1029 chars
[2026-11-04T05:30:25.644Z] [enrich] arxiv.org 98 → 999 chars
[2026-11-04T05:30:25.837Z] [enrich] arxiv.org 75 → 976 chars
[2026-11-04T05:30:26.330Z] [enrich] arxiv.org 105 → 1006 chars
[2026-11-04T05:30:26.447Z] [enrich] arxiv.org 102 → 1003 chars
[2026-11-04T05:30:26.449Z] [enrich] arxiv.org 77 → 978 chars
[2026-11-04T05:30:27.371Z] [enrich] arxiv.org 109 → 1010 chars
[2026-11-04T05:30:27.371Z] Formatting 20 event candidates into the scan table.
[2026-11-04T05:30:29.023Z] [tracker] 8 deadlines tracked
[2026-11-04T05:30:29.024Z] [metrics] events candidates=20 picked=https://firebasehybridaihackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-04T05:30:29.760Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
