---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-390b7fef
created: 2026-10-19T05:33:57.401Z
jobId: 390b7fef-26ce-44c7-b9df-5440a9d4ca17
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-19T05:30:02.229Z
finishedAt: 2026-10-19T05:33:57.401Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-19T05:30:02.229Z
- **Finished:** 2026-10-19T05:33:57.401Z
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
1. ✓ Sweep event sources — `pipeline` (10.4s)
2. ✓ Dedupe + enrich — `pipeline` (10.4s)
3. ✓ Build events table — `pipeline` (234.4s)
4. ✓ Post to Telegram — `pipeline` (235.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-19

⭐ TOP PICK: Band of Agents Hackathon — why it is the one not to miss (TBA prize, TBA deadline) | https://lablab.ai/ai-hackathons/band-of-agents-hackathon

🌍 Band of Agents Hackathon

2 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-19T05:30:02.243Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-19T05:30:02.243Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-19T05:30:10.713Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-19T05:30:12.644Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-19T05:30:12.673Z] [history] 47 URLs posted in last 7d
[2026-10-19T05:30:12.673Z] [history] skip already-posted lablab.ai
[2026-10-19T05:30:12.673Z] [history] skip already-posted gdg.community.dev
[2026-10-19T05:30:12.676Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-10-19T05:30:13.557Z] [enrich] arxiv.org 119 → 770 chars
[2026-10-19T05:30:14.907Z] [enrich] arxiv.org 138 → 1039 chars
[2026-10-19T05:30:14.974Z] [enrich] arxiv.org 163 → 1064 chars
[2026-10-19T05:30:15.770Z] [enrich] arxiv.org 149 → 1050 chars
[2026-10-19T05:30:15.791Z] [enrich] arxiv.org 94 → 995 chars
[2026-10-19T05:30:16.071Z] [enrich] arxiv.org 122 → 1023 chars
[2026-10-19T05:30:16.794Z] [enrich] arxiv.org 105 → 1006 chars
[2026-10-19T05:30:17.175Z] [enrich] arxiv.org 103 → 1004 chars
[2026-10-19T05:30:17.175Z] Formatting 20 event candidates into the scan table.
[2026-10-19T05:33:56.660Z] [tracker] 9 deadlines tracked
[2026-10-19T05:33:56.661Z] [metrics] events candidates=20 picked=https://lablab.ai/ai-hackathons/band-of-agents-hackathon score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-10-19T05:33:57.401Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
