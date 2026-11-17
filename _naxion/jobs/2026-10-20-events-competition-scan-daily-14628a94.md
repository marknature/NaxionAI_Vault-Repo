---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-14628a94
created: 2026-10-20T05:36:14.028Z
jobId: 14628a94-07bd-48bd-9ecb-a7fb69c890cc
status: failed
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-20T05:30:18.987Z
finishedAt: 2026-10-20T05:36:14.028Z
---

# Events & Competition Scan — daily

- **Status:** failed
- **Template:** events-competition-scan
- **Started:** 2026-10-20T05:30:18.987Z
- **Finished:** 2026-10-20T05:36:14.028Z
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
1. ✓ Sweep event sources — `pipeline` (14.7s)
2. ✓ Dedupe + enrich — `pipeline` (14.8s)
3. · Build events table — `pipeline`
4. · Post to Telegram — `pipeline`

## Error
```
terminated
```

<details><summary>Log</summary>

```
[2026-10-20T05:30:19.127Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-20T05:30:19.127Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-20T05:30:23.735Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-20T05:30:33.809Z] [events] web search gathered 16 candidates (quality-filtered).
[2026-10-20T05:30:33.957Z] [history] 50 URLs posted in last 7d
[2026-10-20T05:30:33.957Z] [history] skip already-posted gdg.community.dev
[2026-10-20T05:30:33.961Z] [filter] deduped 24 → 23 (spam/history removed)
[2026-10-20T05:30:34.152Z] [enrich] techcrunch.com 107 → 1008 chars
[2026-10-20T05:30:34.154Z] [enrich] theverge.com 107 → 1008 chars
[2026-10-20T05:30:34.180Z] [enrich] techcrunch.com 123 → 1024 chars
[2026-10-20T05:30:34.191Z] [enrich] techcrunch.com 99 → 1000 chars
[2026-10-20T05:30:34.378Z] [enrich] blogs.nvidia.com 112 → 1013 chars
[2026-10-20T05:30:34.518Z] [enrich] aws.amazon.com 105 → 1006 chars
[2026-10-20T05:30:35.051Z] [enrich] simonwillison.net 57 → 958 chars
[2026-10-20T05:30:36.960Z] [enrich] arstechnica.com 117 → 1018 chars
[2026-10-20T05:30:36.960Z] Formatting 20 event candidates into the scan table.
[2026-10-20T05:36:14.028Z] error: terminated
```
</details>
