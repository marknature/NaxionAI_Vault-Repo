---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-7902dd80
created: 2026-10-21T05:39:10.562Z
jobId: 7902dd80-98fe-4707-b1e4-f1c2409765cc
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-21T05:30:04.261Z
finishedAt: 2026-10-21T05:39:10.562Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-21T05:30:04.261Z
- **Finished:** 2026-10-21T05:39:10.562Z
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
1. ✓ Sweep event sources — `pipeline` (7.5s)
2. ✓ Dedupe + enrich — `pipeline` (7.5s)
3. ✓ Build events table — `pipeline` (546.0s)
4. ✓ Post to Telegram — `pipeline` (546.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-21

⭐ TOP PICK: 2026 AI for Good Hackathon — don't miss this chance to build AI solutions for social good with a non-monetary prize | https://2026ai4goodhackathon.devpost.com/

💻 2026 AI for Good Hackathon

6 free · 4 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-21T05:30:04.271Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-21T05:30:04.272Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-21T05:30:10.985Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-21T05:30:11.760Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-10-21T05:30:11.788Z] [history] 54 URLs posted in last 7d
[2026-10-21T05:30:11.788Z] [history] skip already-posted lablab.ai
[2026-10-21T05:30:11.788Z] [history] skip already-posted lablab.ai
[2026-10-21T05:30:11.788Z] [history] skip already-posted gdg.community.dev
[2026-10-21T05:30:11.791Z] [filter] deduped 22 → 19 (spam/history removed)
[2026-10-21T05:30:12.235Z] [enrich] arxiv.org 131 → 1032 chars
[2026-10-21T05:30:12.429Z] [enrich] arxiv.org 125 → 1026 chars
[2026-10-21T05:30:12.892Z] [enrich] arxiv.org 125 → 1026 chars
[2026-10-21T05:30:13.031Z] [enrich] arxiv.org 106 → 1007 chars
[2026-10-21T05:30:13.445Z] [enrich] arxiv.org 124 → 1025 chars
[2026-10-21T05:30:13.465Z] [enrich] arxiv.org 117 → 1018 chars
[2026-10-21T05:30:13.565Z] [enrich] arxiv.org 91 → 992 chars
[2026-10-21T05:30:13.588Z] [enrich] arxiv.org 95 → 996 chars
[2026-10-21T05:30:13.588Z] Formatting 19 event candidates into the scan table.
[2026-10-21T05:39:10.276Z] [tracker] 8 deadlines tracked
[2026-10-21T05:39:10.278Z] [metrics] events candidates=19 picked=https://2026ai4goodhackathon.devpost.com/ score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-10-21T05:39:10.561Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
