---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-5450ff40
created: 2026-10-29T05:37:47.361Z
jobId: 5450ff40-a71c-4bfa-ae1d-5dc3f1076b0b
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-29T05:37:46.998Z
finishedAt: 2026-10-29T05:37:47.361Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-29T05:37:46.998Z
- **Finished:** 2026-10-29T05:37:47.361Z
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
1. ✓ Sweep event sources — `pipeline` (0.0s)
2. ✓ Dedupe + enrich — `pipeline` (0.2s)
3. · Build events table — `pipeline`
4. · Post to Telegram — `pipeline`

<details><summary>Log</summary>

```
[2026-10-29T05:37:47.093Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-29T05:37:47.093Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-29T05:37:47.328Z] [history] 101 URLs posted in last 7d
[2026-10-29T05:37:47.336Z] No tech events or competitions found today — skipping the post.
[2026-10-29T05:37:47.361Z] [metrics] events candidates=0 picked=none score=? domains=
```
</details>
