---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-1e7ade17
created: 2026-11-20T05:34:57.505Z
jobId: 1e7ade17-7cbb-40ca-82ff-96edd85ff7da
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-20T05:30:21.850Z
finishedAt: 2026-11-20T05:34:57.505Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-20T05:30:21.850Z
- **Finished:** 2026-11-20T05:34:57.505Z
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
1. ✓ Sweep event sources — `pipeline` (24.9s)
2. ✓ Dedupe + enrich — `pipeline` (25.1s)
3. ✓ Build events table — `pipeline` (275.1s)
4. ✓ Post to Telegram — `pipeline` (275.5s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-20

⭐ TOP PICK: TBA | TBA

💻 Hackathon: ZimHack 2026 - A Platform for Zimbabwean Developers to Showcase and Collaborate | https://zimhack.zimtech.org/

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-20T05:30:21.999Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-20T05:30:21.999Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-20T05:30:27.218Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-20T05:30:46.887Z] [events] web search gathered 18 candidates (quality-filtered).
[2026-11-20T05:30:47.058Z] [history] 168 URLs posted in last 7d
[2026-11-20T05:30:47.059Z] [history] skip already-posted support.microsoft.com
[2026-11-20T05:30:47.064Z] [filter] deduped 26 → 25 (spam/history removed)
[2026-11-20T05:30:47.570Z] [enrich] arxiv.org 133 → 1034 chars
[2026-11-20T05:30:48.149Z] [enrich] arxiv.org 103 → 1004 chars
[2026-11-20T05:30:48.168Z] [enrich] arxiv.org 127 → 1028 chars
[2026-11-20T05:30:48.173Z] [enrich] arxiv.org 89 → 990 chars
[2026-11-20T05:30:48.204Z] [enrich] arxiv.org 84 → 985 chars
[2026-11-20T05:30:48.418Z] [enrich] arxiv.org 124 → 1025 chars
[2026-11-20T05:30:48.684Z] [enrich] arxiv.org 102 → 1003 chars
[2026-11-20T05:30:50.436Z] [enrich] support.microsoft.com 125 → 1026 chars
[2026-11-20T05:30:50.437Z] Formatting 20 event candidates into the scan table.
[2026-11-20T05:34:57.145Z] [tracker] 10 deadlines tracked
[2026-11-20T05:34:57.146Z] [metrics] events candidates=20 picked=https://zimhack.zimtech.org/ score=? domains=arxiv.org,arxiv.org,support.microsoft.com,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-20T05:34:57.504Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
