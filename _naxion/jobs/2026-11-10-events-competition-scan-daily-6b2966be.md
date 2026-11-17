---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-6b2966be
created: 2026-11-10T05:36:12.270Z
jobId: 6b2966be-c929-4b15-adae-b27f4cae043d
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-10T05:30:24.270Z
finishedAt: 2026-11-10T05:36:12.268Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-10T05:30:24.270Z
- **Finished:** 2026-11-10T05:36:12.268Z
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
1. ✓ Sweep event sources — `pipeline` (7.6s)
2. ✓ Dedupe + enrich — `pipeline` (7.8s)
3. ✓ Build events table — `pipeline` (347.7s)
4. ✓ Post to Telegram — `pipeline` (348.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-10

⭐ TOP PICK: Ctrl+V Hackathon — win $28,000 in prizes and build with AI to break barriers | https://ctrl-v-hackathon-31831.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

💻 Ctrl+V Hackathon

4 free · 1 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-10T05:30:24.286Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-10T05:30:24.286Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-10T05:30:31.313Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-10T05:30:31.931Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-11-10T05:30:32.027Z] [history] 126 URLs posted in last 7d
[2026-11-10T05:30:32.029Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-10T05:30:32.043Z] [filter] deduped 22 → 21 (spam/history removed)
[2026-11-10T05:30:32.545Z] [enrich] arxiv.org 127 → 1028 chars
[2026-11-10T05:30:32.760Z] [enrich] arxiv.org 156 → 1057 chars
[2026-11-10T05:30:32.770Z] [enrich] arxiv.org 97 → 998 chars
[2026-11-10T05:30:32.848Z] [enrich] arxiv.org 121 → 1022 chars
[2026-11-10T05:30:33.693Z] [enrich] wired.com 95 → 996 chars
[2026-11-10T05:30:38.001Z] [enrich] arxiv.org 126 → 1027 chars
[2026-11-10T05:30:38.005Z] [enrich] arxiv.org 94 → 995 chars
[2026-11-10T05:30:38.128Z] [enrich] arxiv.org 83 → 984 chars
[2026-11-10T05:30:38.128Z] Formatting 20 event candidates into the scan table.
[2026-11-10T05:36:11.959Z] [tracker] 6 deadlines tracked
[2026-11-10T05:36:11.966Z] [metrics] events candidates=20 picked=https://ctrl-v-hackathon-31831.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,wired.com,arxiv.org,arxiv.org
[2026-11-10T05:36:12.267Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
