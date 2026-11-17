---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-c71bb05a
created: 2026-11-11T06:01:08.680Z
jobId: c71bb05a-98a8-4d04-ab04-3eb4dfc07841
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-11T06:00:47.856Z
finishedAt: 2026-11-11T06:01:08.679Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-11T06:00:47.856Z
- **Finished:** 2026-11-11T06:01:08.679Z
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
1. ✓ Sweep event sources — `pipeline` (9.6s)
2. ✓ Dedupe + enrich — `pipeline` (9.7s)
3. · Build events table — `pipeline`
4. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-11T06:00:47.857Z] Queued — 0 tasks ahead (cap 2 running at once).
[2026-11-11T06:00:58.943Z] Started after 11s in the task queue.
[2026-11-11T06:00:58.944Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-11T06:00:58.944Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-11T06:01:08.675Z] [history] 127 URLs posted in last 7d
[2026-11-11T06:01:08.676Z] No tech events or competitions found today — skipping the post.
[2026-11-11T06:01:08.679Z] [metrics] events candidates=0 picked=none score=? domains=
```
</details>
