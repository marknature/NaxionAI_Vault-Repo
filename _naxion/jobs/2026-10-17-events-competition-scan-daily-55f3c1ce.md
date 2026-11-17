---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-55f3c1ce
created: 2026-10-17T06:20:05.275Z
jobId: 55f3c1ce-d9f5-4b3a-ab2f-f77861f8d5cd
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-17T06:12:59.689Z
finishedAt: 2026-10-17T06:20:05.274Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-17T06:12:59.689Z
- **Finished:** 2026-10-17T06:20:05.274Z
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
1. ✓ Sweep event sources — `pipeline` (5.7s)
2. ✓ Dedupe + enrich — `pipeline` (5.8s)
3. ✓ Build events table — `pipeline` (122.8s)
4. ✓ Post to Telegram — `pipeline` (123.5s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-17

⭐ TOP PICK: None — no suitable events found |

0 free · 0 paid · 0 remote global

0 free · 0 paid · 0 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-17T06:12:59.690Z] Queued — 3 tasks ahead (cap 2 running at once).
[2026-10-17T06:18:01.753Z] Started after 302s in the task queue.
[2026-10-17T06:18:01.753Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-17T06:18:01.753Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-17T06:18:06.536Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-17T06:18:07.500Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-17T06:18:07.507Z] [history] 36 URLs posted in last 7d
[2026-10-17T06:18:07.508Z] [history] skip already-posted lablab.ai
[2026-10-17T06:18:07.508Z] [history] skip already-posted lablab.ai
[2026-10-17T06:18:07.508Z] [history] skip already-posted gdg.community.dev
[2026-10-17T06:18:07.513Z] [filter] deduped 23 → 20 (spam/history removed)
[2026-10-17T06:18:07.517Z] [enrich] aws.amazon.com 139 → 1040 chars
[2026-10-17T06:18:07.517Z] [enrich] theverge.com 111 → 1012 chars
[2026-10-17T06:18:07.517Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-17T06:18:07.517Z] [enrich] theverge.com 107 → 1008 chars
[2026-10-17T06:18:07.518Z] [enrich] arstechnica.com 91 → 992 chars
[2026-10-17T06:18:07.518Z] [enrich] simonwillison.net 85 → 986 chars
[2026-10-17T06:18:07.518Z] [enrich] techcrunch.com 81 → 982 chars
[2026-10-17T06:18:07.518Z] [enrich] theverge.com 58 → 959 chars
[2026-10-17T06:18:07.518Z] Formatting 20 event candidates into the scan table.
[2026-10-17T06:20:04.526Z] [tracker] no machine-readable deadlines this run
[2026-10-17T06:20:04.528Z] [metrics] events candidates=20 picked=https://aws.amazon.com/blogs/machine-learning/building-trust-in-ai-agents-a-production-ready-evaluation-framework-with-amazon-bedrock-agentcore/ score=? domains=aws.amazon.com,theverge.com,theverge.com,theverge.com,arstechnica.com,simonwillison.net,techcrunch.com,theverge.com
[2026-10-17T06:20:05.274Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
