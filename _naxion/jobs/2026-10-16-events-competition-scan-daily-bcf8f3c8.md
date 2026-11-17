---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-bcf8f3c8
created: 2026-10-16T05:40:52.566Z
jobId: bcf8f3c8-594e-48d8-98d4-7c3b917a1c81
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-16T05:36:38.606Z
finishedAt: 2026-10-16T05:40:52.565Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-16T05:36:38.606Z
- **Finished:** 2026-10-16T05:40:52.565Z
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
1. ✓ Sweep event sources — `pipeline` (13.2s)
2. ✓ Dedupe + enrich — `pipeline` (13.2s)
3. ✓ Build events table — `pipeline` (253.0s)
4. ✓ Post to Telegram — `pipeline` (254.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-16

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-16T05:36:38.613Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-16T05:36:38.613Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-16T05:36:51.022Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-16T05:36:51.800Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-16T05:36:51.814Z] [history] 29 URLs posted in last 7d
[2026-10-16T05:36:51.815Z] [history] skip already-posted lablab.ai
[2026-10-16T05:36:51.829Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-16T05:36:52.532Z] [enrich] ventureburn.com 85 → 802 chars
[2026-10-16T05:36:52.533Z] [enrich] ventureburn.com 86 → 790 chars
[2026-10-16T05:36:52.533Z] [enrich] ventureburn.com 82 → 804 chars
[2026-10-16T05:36:52.752Z] [enrich] arxiv.org 83 → 984 chars
[2026-10-16T05:36:52.755Z] [enrich] arxiv.org 100 → 1001 chars
[2026-10-16T05:36:54.333Z] [enrich] arxiv.org 116 → 1017 chars
[2026-10-16T05:36:54.335Z] [enrich] arxiv.org 129 → 1030 chars
[2026-10-16T05:36:54.462Z] [enrich] arxiv.org 98 → 999 chars
[2026-10-16T05:36:54.462Z] Formatting 20 event candidates into the scan table.
[2026-10-16T05:40:51.613Z] [tracker] no machine-readable deadlines this run
[2026-10-16T05:40:51.616Z] [metrics] events candidates=20 picked=https://arxiv.org/abs/2610.20669 score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,ventureburn.com,ventureburn.com,arxiv.org,ventureburn.com
[2026-10-16T05:40:52.564Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
