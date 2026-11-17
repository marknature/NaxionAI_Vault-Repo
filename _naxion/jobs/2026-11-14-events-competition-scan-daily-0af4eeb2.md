---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-0af4eeb2
created: 2026-11-14T05:36:06.869Z
jobId: 0af4eeb2-07db-4207-9ebd-24e02af6a4f5
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-14T05:30:04.623Z
finishedAt: 2026-11-14T05:36:06.869Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-14T05:30:04.623Z
- **Finished:** 2026-11-14T05:36:06.869Z
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
1. ✓ Sweep event sources — `pipeline` (24.4s)
2. ✓ Dedupe + enrich — `pipeline` (24.6s)
3. ✓ Build events table — `pipeline` (361.9s)
4. ✓ Post to Telegram — `pipeline` (362.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-14

⭐ TOP PICK: Global Devpost Hackathon - The Future of AI in Healthcare (TBA) | TBA

💡 Why attend: Gain insights and collaborate with global AI experts, learn from real-world healthcare challenges, and win cash prizes and exposure.

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-14T05:30:04.633Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-14T05:30:04.633Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-14T05:30:10.642Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-14T05:30:29.046Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-14T05:30:29.205Z] [history] 145 URLs posted in last 7d
[2026-11-14T05:30:29.626Z] [enrich] arxiv.org 113 → 1014 chars
[2026-11-14T05:30:30.509Z] [enrich] arxiv.org 99 → 1000 chars
[2026-11-14T05:30:30.610Z] [enrich] arxiv.org 97 → 998 chars
[2026-11-14T05:30:30.613Z] [enrich] arxiv.org 113 → 1014 chars
[2026-11-14T05:30:31.008Z] [enrich] arxiv.org 89 → 990 chars
[2026-11-14T05:30:32.150Z] [enrich] microsoft.com 130 → 1031 chars
[2026-11-14T05:30:32.489Z] [enrich] support.microsoft.com 135 → 1036 chars
[2026-11-14T05:30:33.913Z] [enrich] support.microsoft.com 135 → 1036 chars
[2026-11-14T05:30:33.913Z] Formatting 20 event candidates into the scan table.
[2026-11-14T05:36:06.548Z] [tracker] no machine-readable deadlines this run
[2026-11-14T05:36:06.550Z] [metrics] events candidates=20 picked=https://support.microsoft.com/en-gb/windows/how-to-get-help-in-windows-711b6492-0435-0038-8706-7c6b0feb200a score=? domains=support.microsoft.com,support.microsoft.com,microsoft.com,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-14T05:36:06.868Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
