---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-446dd26d
created: 2026-10-14T05:30:38.313Z
jobId: 446dd26d-e159-41e7-a4dc-fdba84475066
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-14T05:30:09.888Z
finishedAt: 2026-10-14T05:30:38.312Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-14T05:30:09.888Z
- **Finished:** 2026-10-14T05:30:38.312Z
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
1. ✓ Sweep event sources — `pipeline` (5.2s)
2. ✓ Dedupe + enrich — `pipeline` (5.3s)
3. ✓ Build events table — `pipeline` (28.1s)
4. ✓ Post to Telegram — `pipeline` (28.4s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-14

⭐ TOP PICK: MLAI Hackathon 2026 — High-visibility AI application challenge with a tight 2-day window | https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 MLAI Hackathon 2026

1 free · 1 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-14T05:30:09.903Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-14T05:30:09.903Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-14T05:30:14.898Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-14T05:30:15.119Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-14T05:30:15.147Z] [history] 33 URLs posted in last 7d
[2026-10-14T05:30:15.148Z] [history] skip already-posted agentsforhumans.devpost.com
[2026-10-14T05:30:15.160Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-14T05:30:15.294Z] [enrich] techcrunch.com 126 → 1027 chars
[2026-10-14T05:30:15.298Z] [enrich] techcrunch.com 122 → 1023 chars
[2026-10-14T05:30:22.192Z] [enrich] simonwillison.net 69 → 970 chars
[2026-10-14T05:30:22.259Z] [enrich] ventureburn.com 88 → 799 chars
[2026-10-14T05:30:22.490Z] [enrich] wired.com 114 → 1015 chars
[2026-10-14T05:30:27.444Z] [enrich] deepmind.google 131 → 1032 chars
[2026-10-14T05:30:28.774Z] [enrich] techcrunch.com 103 → 1004 chars
[2026-10-14T05:30:32.204Z] [enrich] arstechnica.com 103 → 1004 chars
[2026-10-14T05:30:32.204Z] Formatting 20 event candidates into the scan table.
[2026-10-14T05:30:37.980Z] [tracker] 4 deadlines tracked
[2026-10-14T05:30:37.982Z] [metrics] events candidates=20 picked=https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=deepmind.google,techcrunch.com,techcrunch.com,wired.com,techcrunch.com,arstechnica.com,ventureburn.com,simonwillison.net
[2026-10-14T05:30:38.312Z] Posted Events & Competition Scan to Telegram chat -1004307136262.
```
</details>
