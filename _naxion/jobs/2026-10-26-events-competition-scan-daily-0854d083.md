---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-0854d083
created: 2026-10-26T05:45:28.953Z
jobId: 0854d083-14b1-400f-9709-549ba609a441
status: failed
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-26T05:30:17.787Z
finishedAt: 2026-10-26T05:45:28.953Z
---

# Events & Competition Scan — daily

- **Status:** failed
- **Template:** events-competition-scan
- **Started:** 2026-10-26T05:30:17.787Z
- **Finished:** 2026-10-26T05:45:28.953Z
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
1. ✓ Sweep event sources — `pipeline` (6.5s)
2. ✓ Dedupe + enrich — `pipeline` (6.5s)
3. · Build events table — `pipeline`
4. · Post to Telegram — `pipeline`

## Error
```
This operation was aborted
```

<details><summary>Log</summary>

```
[2026-10-26T05:30:17.794Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-26T05:30:17.795Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-26T05:30:23.560Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-26T05:30:24.268Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-26T05:30:24.301Z] [history] 80 URLs posted in last 7d
[2026-10-26T05:30:24.302Z] [history] skip already-posted lablab.ai
[2026-10-26T05:30:24.302Z] [history] skip already-posted lablab.ai
[2026-10-26T05:30:24.304Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-10-26T05:30:24.743Z] [enrich] arxiv.org 87 → 988 chars
[2026-10-26T05:30:24.786Z] [enrich] arxiv.org 138 → 1039 chars
[2026-10-26T05:30:24.999Z] [enrich] arxiv.org 125 → 1026 chars
[2026-10-26T05:30:25.216Z] [enrich] arxiv.org 99 → 1000 chars
[2026-10-26T05:30:25.466Z] [enrich] arxiv.org 107 → 1008 chars
[2026-10-26T05:30:26.170Z] [enrich] arxiv.org 123 → 1024 chars
[2026-10-26T05:30:26.171Z] [enrich] arxiv.org 98 → 999 chars
[2026-10-26T05:30:26.339Z] [enrich] arxiv.org 107 → 1008 chars
[2026-10-26T05:30:26.339Z] Formatting 20 event candidates into the scan table.
[2026-10-26T05:45:28.953Z] error: This operation was aborted
```
</details>
