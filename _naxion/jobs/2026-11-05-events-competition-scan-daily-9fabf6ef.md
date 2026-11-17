---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-9fabf6ef
created: 2026-11-05T05:30:30.303Z
jobId: 9fabf6ef-ca60-4aaf-b54d-49f062fdeeb1
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-05T05:30:15.836Z
finishedAt: 2026-11-05T05:30:30.302Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-05T05:30:15.836Z
- **Finished:** 2026-11-05T05:30:30.302Z
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
1. ✓ Sweep event sources — `pipeline` (8.5s)
2. ✓ Dedupe + enrich — `pipeline` (8.6s)
3. ✓ Build events table — `pipeline` (13.8s)
4. ✓ Post to Telegram — `pipeline` (14.5s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-05

⭐ TOP PICK: DevFest Harare 2026 — High-visibility networking for Zimbabwe's tech ecosystem in the Agentic Era | https://sessionize.com/devfest-harare-2026/

🎪 DevFest Harare 2026

3 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-05T05:30:15.843Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-05T05:30:15.843Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-05T05:30:21.031Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-05T05:30:24.388Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-05T05:30:24.412Z] [history] 114 URLs posted in last 7d
[2026-11-05T05:30:24.413Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-05T05:30:24.413Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-11-05T05:30:24.413Z] [history] skip already-posted lablab.ai
[2026-11-05T05:30:24.415Z] [filter] deduped 23 → 20 (spam/history removed)
[2026-11-05T05:30:24.780Z] [enrich] arxiv.org 125 → 1026 chars
[2026-11-05T05:30:25.025Z] [enrich] arxiv.org 90 → 991 chars
[2026-11-05T05:30:25.034Z] [enrich] arxiv.org 119 → 1020 chars
[2026-11-05T05:30:25.523Z] [enrich] arxiv.org 126 → 1027 chars
[2026-11-05T05:30:25.646Z] [enrich] arxiv.org 125 → 1026 chars
[2026-11-05T05:30:26.233Z] [enrich] arxiv.org 92 → 993 chars
[2026-11-05T05:30:26.691Z] [enrich] arxiv.org 106 → 1007 chars
[2026-11-05T05:30:27.204Z] [enrich] arxiv.org 120 → 1021 chars
[2026-11-05T05:30:27.204Z] Formatting 20 event candidates into the scan table.
[2026-11-05T05:30:29.604Z] [tracker] 9 deadlines tracked
[2026-11-05T05:30:29.606Z] [metrics] events candidates=20 picked=https://sessionize.com/devfest-harare-2026/ score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-05T05:30:30.302Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
