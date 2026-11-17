---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-8df479e6
created: 2026-10-22T05:40:11.572Z
jobId: 8df479e6-404d-4a9e-b341-3a92eb6a9c97
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-22T05:30:20.389Z
finishedAt: 2026-10-22T05:40:11.569Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-22T05:30:20.389Z
- **Finished:** 2026-10-22T05:40:11.569Z
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
1. ✓ Sweep event sources — `pipeline` (6.6s)
2. ✓ Dedupe + enrich — `pipeline` (6.8s)
3. ✓ Build events table — `pipeline` (590.5s)
4. ✓ Post to Telegram — `pipeline` (591.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-22

⭐ TOP PICK: NVIDIA Open Models Power a New Wave of European Public Sector Projects — why it is the one not to miss (prize/deadline hook) | https://blogs.nvidia.com/blog/european-public-sector-open-models/

💻 2026 AI for Good Hackathon

9 free · 1 paid · 0 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-22T05:30:20.404Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-22T05:30:20.404Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-22T05:30:25.669Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-22T05:30:27.042Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-22T05:30:27.196Z] [history] 57 URLs posted in last 7d
[2026-10-22T05:30:27.197Z] [history] skip already-posted lablab.ai
[2026-10-22T05:30:27.197Z] [history] skip already-posted gdg.community.dev
[2026-10-22T05:30:27.201Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-10-22T05:30:27.536Z] [enrich] blogs.nvidia.com 134 → 1035 chars
[2026-10-22T05:30:27.871Z] [enrich] blogs.nvidia.com 99 → 1000 chars
[2026-10-22T05:30:27.996Z] [enrich] blogs.nvidia.com 130 → 1031 chars
[2026-10-22T05:30:28.148Z] [enrich] blogs.nvidia.com 107 → 1008 chars
[2026-10-22T05:30:28.605Z] [enrich] arxiv.org 124 → 1025 chars
[2026-10-22T05:30:29.313Z] [enrich] arxiv.org 125 → 1026 chars
[2026-10-22T05:30:29.411Z] [enrich] blogs.nvidia.com 91 → 992 chars
[2026-10-22T05:30:29.713Z] [enrich] blogs.nvidia.com 97 → 998 chars
[2026-10-22T05:30:29.713Z] Formatting 20 event candidates into the scan table.
[2026-10-22T05:40:10.854Z] [tracker] 7 deadlines tracked
[2026-10-22T05:40:10.859Z] [metrics] events candidates=20 picked=https://blogs.nvidia.com/blog/european-public-sector-open-models/ score=? domains=blogs.nvidia.com,blogs.nvidia.com,arxiv.org,arxiv.org,blogs.nvidia.com,blogs.nvidia.com,blogs.nvidia.com,blogs.nvidia.com
[2026-10-22T05:40:11.569Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
