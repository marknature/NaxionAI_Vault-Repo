---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-1ba38e35
created: 2026-10-13T05:30:30.059Z
jobId: 1ba38e35-591b-43a0-8728-77843ff2ec65
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-13T05:30:11.021Z
finishedAt: 2026-10-13T05:30:30.059Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-13T05:30:11.021Z
- **Finished:** 2026-10-13T05:30:30.059Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
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
1. ✓ Sweep event sources — `pipeline` (6.0s)
2. ✓ Dedupe + enrich — `pipeline` (6.0s)
3. ✓ Build events table — `pipeline` (18.7s)
4. ✓ Post to Telegram — `pipeline` (19.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-13

⭐ TOP PICK: MLAI Hackathon 2026 — High-visibility AI application challenge with a tight 3-day window | https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 MLAI Hackathon 2026

1 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-13T05:30:11.025Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-13T05:30:11.025Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-13T05:30:16.175Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-13T05:30:17.039Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-13T05:30:17.051Z] [history] 31 URLs posted in last 7d
[2026-10-13T05:30:17.052Z] [history] skip already-posted agentsforhumans.devpost.com
[2026-10-13T05:30:17.055Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-13T05:30:17.526Z] [enrich] arxiv.org 170 → 1071 chars
[2026-10-13T05:30:17.637Z] [enrich] blogs.nvidia.com 114 → 1015 chars
[2026-10-13T05:30:22.293Z] [enrich] arxiv.org 167 → 1068 chars
[2026-10-13T05:30:22.351Z] [enrich] arxiv.org 100 → 1001 chars
[2026-10-13T05:30:22.618Z] [enrich] arxiv.org 101 → 1002 chars
[2026-10-13T05:30:22.636Z] [enrich] arxiv.org 92 → 993 chars
[2026-10-13T05:30:22.636Z] [enrich] arxiv.org 115 → 1016 chars
[2026-10-13T05:30:22.646Z] [enrich] arxiv.org 129 → 1030 chars
[2026-10-13T05:30:22.646Z] Formatting 20 event candidates into the scan table.
[2026-10-13T05:30:29.769Z] [tracker] 4 deadlines tracked
[2026-10-13T05:30:29.770Z] [metrics] events candidates=20 picked=https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,blogs.nvidia.com,arxiv.org,arxiv.org,arxiv.org
[2026-10-13T05:30:30.059Z] Posted Events & Competition Scan to Telegram chat -1004307136262.
```
</details>
