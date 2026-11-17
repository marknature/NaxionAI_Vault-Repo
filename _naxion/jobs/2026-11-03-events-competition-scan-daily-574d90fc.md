---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-574d90fc
created: 2026-11-03T05:30:19.326Z
jobId: 574d90fc-06da-4de5-8dbb-6b4c638794da
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-03T05:30:07.305Z
finishedAt: 2026-11-03T05:30:19.325Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-03T05:30:07.305Z
- **Finished:** 2026-11-03T05:30:19.325Z
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
1. ✓ Sweep event sources — `pipeline` (7.3s)
2. ✓ Dedupe + enrich — `pipeline` (7.3s)
3. ✓ Build events table — `pipeline` (11.4s)
4. ✓ Post to Telegram — `pipeline` (12.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-03

⭐ TOP PICK: STEMergent Hacks 2026 — Best entry point for students to build community-focused AI solutions before the mid-month cutoff | https://stemergent-hacks.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🎪 DevFest Harare 2026

3 free · 0 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-03T05:30:07.314Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-03T05:30:07.314Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-03T05:30:11.859Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-03T05:30:14.599Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-03T05:30:14.619Z] [history] 106 URLs posted in last 7d
[2026-11-03T05:30:14.620Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-03T05:30:14.620Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-11-03T05:30:14.620Z] [history] skip already-posted lablab.ai
[2026-11-03T05:30:14.620Z] [history] skip already-posted lablab.ai
[2026-11-03T05:30:14.622Z] [filter] deduped 23 → 18 (spam/history removed)
[2026-11-03T05:30:14.800Z] [enrich] techcrunch.com 112 → 1013 chars
[2026-11-03T05:30:14.827Z] [enrich] techcrunch.com 121 → 1022 chars
[2026-11-03T05:30:14.833Z] [enrich] techcrunch.com 122 → 1023 chars
[2026-11-03T05:30:14.860Z] [enrich] theverge.com 109 → 1010 chars
[2026-11-03T05:30:14.900Z] [enrich] technologyreview.com 112 → 1013 chars
[2026-11-03T05:30:15.035Z] [enrich] techcrunch.com 112 → 1013 chars
[2026-11-03T05:30:15.734Z] [enrich] arstechnica.com 90 → 991 chars
[2026-11-03T05:30:15.984Z] [enrich] devpost.com 600 → 1100 chars
[2026-11-03T05:30:15.984Z] Formatting 18 event candidates into the scan table.
[2026-11-03T05:30:18.666Z] [tracker] 7 deadlines tracked
[2026-11-03T05:30:18.668Z] [metrics] events candidates=18 picked=https://stemergent-hacks.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=techcrunch.com,techcrunch.com,technologyreview.com,techcrunch.com,techcrunch.com,theverge.com,arstechnica.com,devpost.com
[2026-11-03T05:30:19.324Z] Telegram post failed: telegram send failed: fetch failed
```
</details>
