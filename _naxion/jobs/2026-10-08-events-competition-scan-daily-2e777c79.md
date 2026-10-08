---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-2e777c79
created: 2026-10-08T05:30:44.280Z
jobId: 2e777c79-1fa2-4cd9-bc07-0795df5d2dfe
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-08T05:30:10.031Z
finishedAt: 2026-10-08T05:30:44.279Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-08T05:30:10.031Z
- **Finished:** 2026-10-08T05:30:44.279Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (10.9s)
2. ✓ Dedupe + enrich — `pipeline` (10.9s)
3. ✓ Build events table — `pipeline` (33.5s)
4. ✓ Post to Telegram — `pipeline` (34.2s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-08

Africa Startup Congress 2027 National Pitch Competitions and Roadshows | 2027 | Pan

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-08T05:30:10.039Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-08T05:30:10.039Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-08T05:30:15.358Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-10-08T05:30:20.964Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-08T05:30:20.969Z] [history] 6 URLs posted in last 7d
[2026-10-08T05:30:21.404Z] [enrich] arxiv.org 112 → 1013 chars
[2026-10-08T05:30:21.405Z] [enrich] arxiv.org 124 → 1025 chars
[2026-10-08T05:30:26.678Z] [enrich] arxiv.org 140 → 1041 chars
[2026-10-08T05:30:26.680Z] [enrich] arxiv.org 110 → 1011 chars
[2026-10-08T05:30:26.682Z] [enrich] arxiv.org 143 → 1044 chars
[2026-10-08T05:30:26.761Z] [enrich] arxiv.org 117 → 1018 chars
[2026-10-08T05:30:26.761Z] Formatting 14 event candidates into the scan table.
[2026-10-08T05:30:43.505Z] [metrics] events candidates=14 picked=https://arxiv.org/abs/2610.06971 score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-10-08T05:30:44.279Z] Posted Events & Competition Scan to Telegram chat -1004307136262.
```
</details>
