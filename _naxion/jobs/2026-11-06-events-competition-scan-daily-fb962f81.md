---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-fb962f81
created: 2026-11-06T05:30:29.983Z
jobId: fb962f81-7267-4659-a039-bed2467580b5
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-06T05:30:18.855Z
finishedAt: 2026-11-06T05:30:29.982Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-06T05:30:18.855Z
- **Finished:** 2026-11-06T05:30:29.982Z
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
1. ✓ Sweep event sources — `pipeline` (5.0s)
2. ✓ Dedupe + enrich — `pipeline` (5.1s)
3. ✓ Build events table — `pipeline` (10.0s)
4. ✓ Post to Telegram — `pipeline` (11.1s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-06

⭐ TOP PICK: UGREEN Hackathon 2026 on AI NAS — $46,000 prize pool for AI NAS innovation | https://ugreenhackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 UGREEN Hackathon 2026 on AI NAS

2 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-06T05:30:18.874Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-06T05:30:18.875Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-06T05:30:23.527Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-06T05:30:23.882Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-06T05:30:23.945Z] [history] 114 URLs posted in last 7d
[2026-11-06T05:30:23.947Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-06T05:30:23.948Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-11-06T05:30:23.948Z] [history] skip already-posted lablab.ai
[2026-11-06T05:30:23.948Z] [history] skip already-posted sessionize.com
[2026-11-06T05:30:23.963Z] [filter] deduped 23 → 19 (spam/history removed)
[2026-11-06T05:30:24.713Z] [enrich] arxiv.org 154 → 1055 chars
[2026-11-06T05:30:24.778Z] [enrich] arxiv.org 157 → 1058 chars
[2026-11-06T05:30:25.602Z] [enrich] arxiv.org 122 → 1023 chars
[2026-11-06T05:30:25.624Z] [enrich] arxiv.org 90 → 991 chars
[2026-11-06T05:30:26.137Z] [enrich] arxiv.org 120 → 1021 chars
[2026-11-06T05:30:26.216Z] [enrich] arxiv.org 116 → 1017 chars
[2026-11-06T05:30:26.217Z] [enrich] arxiv.org 116 → 1017 chars
[2026-11-06T05:30:26.360Z] [enrich] arxiv.org 117 → 1018 chars
[2026-11-06T05:30:26.361Z] Formatting 19 event candidates into the scan table.
[2026-11-06T05:30:28.832Z] [tracker] 10 deadlines tracked
[2026-11-06T05:30:28.837Z] [metrics] events candidates=19 picked=https://ugreenhackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-06T05:30:29.981Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
