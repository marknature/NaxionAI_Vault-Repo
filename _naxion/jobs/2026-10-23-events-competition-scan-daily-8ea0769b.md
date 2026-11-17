---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-8ea0769b
created: 2026-10-23T05:37:23.159Z
jobId: 8ea0769b-a37c-494f-b01d-84e566b14fa5
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-23T05:30:07.308Z
finishedAt: 2026-10-23T05:37:23.159Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-23T05:30:07.308Z
- **Finished:** 2026-10-23T05:37:23.159Z
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
1. ✓ Sweep event sources — `pipeline` (8.6s)
2. ✓ Dedupe + enrich — `pipeline` (8.6s)
3. ✓ Build events table — `pipeline` (435.1s)
4. ✓ Post to Telegram — `pipeline` (435.8s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-23

⭐ TOP PICK: UGREEN Hackathon 2026 on AI NAS — don't miss the chance to win $46,000 in prizes and gain valuable experience in AI development | https://ugreenhackathon.devpost.com/

💻 UGREEN Hackathon 2026 on AI NAS

7 free · 3 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-23T05:30:07.315Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-23T05:30:07.315Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-23T05:30:12.300Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-23T05:30:15.899Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-23T05:30:15.923Z] [history] 66 URLs posted in last 7d
[2026-10-23T05:30:15.924Z] [history] skip already-posted lablab.ai
[2026-10-23T05:30:15.924Z] [history] skip already-posted gdg.community.dev
[2026-10-23T05:30:15.926Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-10-23T05:30:16.274Z] [enrich] arxiv.org 113 → 1014 chars
[2026-10-23T05:30:16.543Z] [enrich] arxiv.org 102 → 1003 chars
[2026-10-23T05:30:16.627Z] [enrich] ventureburn.com 119 → 644 chars
[2026-10-23T05:30:16.974Z] [enrich] arxiv.org 122 → 1023 chars
[2026-10-23T05:30:17.020Z] [enrich] arxiv.org 109 → 1010 chars
[2026-10-23T05:30:17.563Z] [enrich] arxiv.org 120 → 1021 chars
[2026-10-23T05:30:17.564Z] [enrich] arxiv.org 124 → 1025 chars
[2026-10-23T05:30:17.767Z] [enrich] arxiv.org 128 → 1029 chars
[2026-10-23T05:30:17.767Z] Formatting 20 event candidates into the scan table.
[2026-10-23T05:37:22.451Z] [tracker] 7 deadlines tracked
[2026-10-23T05:37:22.456Z] [metrics] events candidates=20 picked=https://ugreenhackathon.devpost.com/ score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,ventureburn.com,arxiv.org,arxiv.org,arxiv.org
[2026-10-23T05:37:23.159Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
