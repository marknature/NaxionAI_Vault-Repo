---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-0687d5b7
created: 2026-11-07T10:41:32.928Z
jobId: 0687d5b7-d44f-4c68-b8ec-39a7b1887dc5
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-07T05:36:53.686Z
finishedAt: 2026-11-07T10:41:32.927Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-07T05:36:53.686Z
- **Finished:** 2026-11-07T10:41:32.927Z
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
1. ✓ Sweep event sources — `pipeline` (18279.2s)
2. ✓ Dedupe + enrich — `pipeline` (18279.2s)
3. · Build events table — `pipeline`
4. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-11-07T05:36:53.696Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-07T05:36:53.696Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-07T10:41:32.923Z] [history] 119 URLs posted in last 7d
[2026-11-07T10:41:32.925Z] No tech events or competitions found today — skipping the post.
[2026-11-07T10:41:32.927Z] [metrics] events candidates=0 picked=none score=? domains=
```
</details>
