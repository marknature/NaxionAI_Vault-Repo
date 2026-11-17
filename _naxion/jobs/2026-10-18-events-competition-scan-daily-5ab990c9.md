---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-5ab990c9
created: 2026-10-18T05:32:13.639Z
jobId: 5ab990c9-895c-483a-8e9b-9ba642f5dd51
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-18T05:30:02.864Z
finishedAt: 2026-10-18T05:32:13.639Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-18T05:30:02.864Z
- **Finished:** 2026-10-18T05:32:13.639Z
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
1. ✓ Sweep event sources — `pipeline` (11.8s)
2. ✓ Dedupe + enrich — `pipeline` (11.8s)
3. ✓ Build events table — `pipeline` (130.1s)
4. ✓ Post to Telegram — `pipeline` (130.8s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-18

⭐ TOP PICK: Qloo Agentic Hackathon — win $25,000 in prizes, ends Oct 30 (12 days left) | https://qloo.devpost.com/?ref_feature=challenge&ref_medium=discover

💻 Qloo Agentic Hackathon (Qloo)

2 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-18T05:30:02.882Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-18T05:30:02.882Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-18T05:30:09.346Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-10-18T05:30:14.645Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-18T05:30:14.672Z] [history] 40 URLs posted in last 7d
[2026-10-18T05:30:14.672Z] [history] skip already-posted lablab.ai
[2026-10-18T05:30:14.672Z] [history] skip already-posted lablab.ai
[2026-10-18T05:30:14.672Z] [history] skip already-posted gdg.community.dev
[2026-10-18T05:30:14.675Z] [filter] deduped 22 → 19 (spam/history removed)
[2026-10-18T05:30:14.871Z] [enrich] theverge.com 61 → 962 chars
[2026-10-18T05:30:14.873Z] [enrich] theverge.com 82 → 983 chars
[2026-10-18T05:30:14.895Z] [enrich] theverge.com 87 → 988 chars
[2026-10-18T05:30:15.455Z] [enrich] blogs.nvidia.com 89 → 990 chars
[2026-10-18T05:30:15.646Z] [enrich] techcrunch.com 118 → 1019 chars
[2026-10-18T05:30:15.663Z] [enrich] simonwillison.net 75 → 976 chars
[2026-10-18T05:30:16.773Z] [enrich] techcrunch.com 96 → 997 chars
[2026-10-18T05:30:22.667Z] [enrich] techcrunch.com 85 → 986 chars
[2026-10-18T05:30:22.667Z] Formatting 19 event candidates into the scan table.
[2026-10-18T05:32:12.941Z] [tracker] 8 deadlines tracked
[2026-10-18T05:32:12.944Z] [metrics] events candidates=19 picked=https://qloo.devpost.com/?ref_feature=challenge&ref_medium=discover score=? domains=techcrunch.com,techcrunch.com,blogs.nvidia.com,theverge.com,techcrunch.com,theverge.com,simonwillison.net,theverge.com
[2026-10-18T05:32:13.639Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
