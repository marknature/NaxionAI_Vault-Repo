---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-2b9813e4
created: 2026-11-12T05:34:39.995Z
jobId: 2b9813e4-4ea2-4b3d-a7f6-f63b9d06a0f6
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-12T05:30:29.713Z
finishedAt: 2026-11-12T05:34:39.993Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-12T05:30:29.713Z
- **Finished:** 2026-11-12T05:34:39.993Z
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
1. ✓ Sweep event sources — `pipeline` (9.8s)
2. ✓ Dedupe + enrich — `pipeline` (9.9s)
3. ✓ Build events table — `pipeline` (250.0s)
4. ✓ Post to Telegram — `pipeline` (250.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-12

⭐ TOP PICK: Global AI Hackathon by Devpost · Lablab.ai (https://devpost.com/hackathons/global-ai-hackathon) — Build innovative AI solutions for social impact in 48 hours | Oct 30 (23 days left) | Free | 🔗 [Register]

🚀 Global AI Hackathon by Devpost · Lablab.ai

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-12T05:30:29.723Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-12T05:30:29.723Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-12T05:30:36.542Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-12T05:30:39.541Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-12T05:30:39.589Z] [history] 133 URLs posted in last 7d
[2026-11-12T05:30:39.764Z] [enrich] techcrunch.com 110 → 1011 chars
[2026-11-12T05:30:39.846Z] [enrich] techcrunch.com 75 → 976 chars
[2026-11-12T05:30:39.968Z] [enrich] aws.amazon.com 122 → 1023 chars
[2026-11-12T05:30:40.186Z] [enrich] techcrunch.com 100 → 1001 chars
[2026-11-12T05:30:40.275Z] [enrich] aws.amazon.com 98 → 999 chars
[2026-11-12T05:30:41.300Z] [enrich] aws.amazon.com 101 → 1002 chars
[2026-11-12T05:30:46.112Z] [enrich] openai.com 79 → 980 chars
[2026-11-12T05:30:47.577Z] [enrich] explore.microsoft.com 134 → 1035 chars
[2026-11-12T05:30:47.577Z] Formatting 20 event candidates into the scan table.
[2026-11-12T05:34:39.712Z] [tracker] 7 deadlines tracked
[2026-11-12T05:34:39.715Z] [metrics] events candidates=20 picked=https://devpost.com/hackathons/global-ai-hackathon score=? domains=explore.microsoft.com,aws.amazon.com,techcrunch.com,aws.amazon.com,techcrunch.com,aws.amazon.com,openai.com,techcrunch.com
[2026-11-12T05:34:39.993Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
