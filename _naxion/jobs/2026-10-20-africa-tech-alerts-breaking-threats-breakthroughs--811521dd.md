---
type: job
title: Africa Tech Alerts — BREAKING (threats & breakthroughs)
slug: africa-tech-alerts-breaking-threats-breakthroughs--811521dd
created: 2026-10-20T10:33:56.687Z
jobId: 811521dd-fa78-4722-acef-5f4204732bcb
status: failed
template: africa-tech-alerts
persona: naxie
personaName: Naxie
startedAt: 2026-10-20T10:30:13.511Z
finishedAt: 2026-10-20T10:33:56.687Z
---

# Africa Tech Alerts — BREAKING (threats & breakthroughs)

- **Status:** failed
- **Template:** africa-tech-alerts
- **Started:** 2026-10-20T10:30:13.511Z
- **Finished:** 2026-10-20T10:33:56.687Z
- **Title:** Africa Tech Alerts — BREAKING (threats & breakthroughs)

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep threats + breakthroughs — `pipeline` (188.7s)
2. ✓ Dedupe + enrich — `pipeline` (188.9s)
3. ✓ Quality rank — `pipeline` (222.8s)
4. · Build alerts card — `pipeline`
5. · Post to Telegram — `pipeline`

## Error
```
OpenRouter 404: {"error":{"message":"Provider returned error","code":404,"metadata":{"raw":"{\"status\":404,\"title\":\"Not Found\",\"detail\":\"Function 'ac74040f-9fc9-4c5e-ac74-279ba5161d69': Not found for account 'sxpm0VR-knE2_K2__i14ZbzmXEludXpJbFGRvrvc08w'\"}","provider_name":"Nvidia","is_byok":false}},"user_id":"user_3IGs05w2W5BHHvEfj6ix5N7K85v"}
```

<details><summary>Log</summary>

```
[2026-10-20T10:30:13.519Z] Sweeping for dangerous or amazing tech in, around and to Africa.
[2026-10-20T10:30:13.519Z] [alerts] quality pipeline: RSS (≤48h) + threat/breakthrough search → dedupe → enrich → quality rank
[2026-10-20T10:33:22.263Z] [alerts] web search gathered 15 candidates (quality-filtered).
[2026-10-20T10:33:22.432Z] [history] 54 URLs posted in last 7d
[2026-10-20T10:33:22.433Z] [history] skip already-posted interpol.int
[2026-10-20T10:33:22.433Z] [history] skip already-posted transunionafrica.com
[2026-10-20T10:33:22.433Z] [history] skip already-posted transunion.co.za
[2026-10-20T10:33:22.435Z] [filter] deduped 15 → 12 (spam/history removed)
[2026-10-20T10:33:45.700Z] [enrich] fas.org 162 → 1063 chars
[2026-10-20T10:33:51.331Z] [enrich] facebook.com 148 → 1049 chars
[2026-10-20T10:33:51.748Z] [enrich] aiforafricans.org 367 → 1100 chars
[2026-10-20T10:33:53.948Z] [enrich] laserlightcomms.com 155 → 1056 chars
[2026-10-20T10:33:54.541Z] [enrich] hai.stanford.edu 159 → 1060 chars
[2026-10-20T10:33:55.526Z] [enrich] af.net 600 → 1100 chars
[2026-10-20T10:33:56.321Z] [quality] scoring skipped: OpenRouter 404: {"error":{"message":"Provider returned error","code":404,"metada — keeping authority-sorted order
[2026-10-20T10:33:56.322Z] Picked 12 fresh candidates (top score 5) — drafting the daily card.
[2026-10-20T10:33:56.687Z] error: OpenRouter 404: {"error":{"message":"Provider returned error","code":404,"metadata":{"raw":"{\"status\":404,\"title\":\"Not Found\",\"detail\":\"Function 'ac74040f-9fc9-4c5e-ac74-279ba5161d69': Not found for account 'sxpm0VR-knE2_K2__i14ZbzmXEludXpJbFGRvrvc08w'\"}","provider_name":"Nvidia","is_byok":false}},"user_id":"user_3IGs05w2W5BHHvEfj6ix5N7K85v"}
```
</details>
