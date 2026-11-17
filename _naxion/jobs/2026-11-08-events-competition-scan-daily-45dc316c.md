---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-45dc316c
created: 2026-11-08T05:30:44.936Z
jobId: 45dc316c-d998-4781-b7ef-b671b0ad45f6
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-08T05:30:24.677Z
finishedAt: 2026-11-08T05:30:44.935Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-08T05:30:24.677Z
- **Finished:** 2026-11-08T05:30:44.935Z
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
1. ✓ Sweep event sources — `pipeline` (5.1s)
2. ✓ Dedupe + enrich — `pipeline` (5.1s)
3. ✓ Build events table — `pipeline` (20.0s)
4. ✓ Post to Telegram — `pipeline` (20.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-08

⭐ TOP PICK: #BuildHybridAI 2026 — High-stakes AI development with $30,000 in prizes | https://firebasehybridaihackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 #BuildHybridAI 2026

1 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-08T05:30:24.683Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-08T05:30:24.683Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-08T05:30:29.362Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-08T05:30:29.741Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-08T05:30:29.759Z] [history] 119 URLs posted in last 7d
[2026-11-08T05:30:29.759Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-08T05:30:29.759Z] [history] skip already-posted lablab.ai
[2026-11-08T05:30:29.759Z] [history] skip already-posted lablab.ai
[2026-11-08T05:30:29.762Z] [filter] deduped 23 → 20 (spam/history removed)
[2026-11-08T05:30:29.810Z] [enrich] theverge.com 115 → 1016 chars
[2026-11-08T05:30:29.827Z] [enrich] techcrunch.com 113 → 1014 chars
[2026-11-08T05:30:29.905Z] [enrich] techcrunch.com 104 → 1005 chars
[2026-11-08T05:30:30.168Z] [enrich] simonwillison.net 112 → 1013 chars
[2026-11-08T05:30:32.043Z] [enrich] iafrica.com 77 → 978 chars
[2026-11-08T05:30:34.877Z] [enrich] iafrica.com 113 → 1014 chars
[2026-11-08T05:30:41.758Z] [enrich] iafrica.com 92 → 993 chars
[2026-11-08T05:30:42.570Z] [enrich] iafrica.com 110 → 1011 chars
[2026-11-08T05:30:42.570Z] Formatting 20 event candidates into the scan table.
[2026-11-08T05:30:44.663Z] [tracker] 5 deadlines tracked
[2026-11-08T05:30:44.664Z] [metrics] events candidates=20 picked=https://firebasehybridaihackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=theverge.com,techcrunch.com,iafrica.com,simonwillison.net,iafrica.com,techcrunch.com,iafrica.com,iafrica.com
[2026-11-08T05:30:44.935Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
