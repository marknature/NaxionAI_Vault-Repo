---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-13c3426b
created: 2026-10-28T19:53:44.405Z
jobId: 13c3426b-bd79-48f5-81fa-5fb2aa08bd33
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-28T19:14:25.727Z
finishedAt: 2026-10-28T19:53:44.405Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-28T19:14:25.727Z
- **Finished:** 2026-10-28T19:53:44.405Z
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
1. ✓ Sweep event sources — `pipeline` (8.5s)
2. ✓ Dedupe + enrich — `pipeline` (8.5s)
3. ✓ Build events table — `pipeline` (569.1s)
4. ✓ Post to Telegram — `pipeline` (569.4s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-28

⭐ TOP PICK: PayPal AI Hackathon — win up to $100,000 in cash prizes and get exposure to PayPal's AI ecosystem | https://paypalaihackathon.devpost.com/

💻 Qloo Agentic Hackathon

5 free · 1 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-28T19:14:25.728Z] Queued — 4 tasks ahead (cap 2 running at once).
[2026-10-28T19:44:15.022Z] Started after 1789s in the task queue.
[2026-10-28T19:44:15.023Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-28T19:44:15.023Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-28T19:44:19.892Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-10-28T19:44:23.477Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-28T19:44:23.499Z] [history] 96 URLs posted in last 7d
[2026-10-28T19:44:23.499Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-10-28T19:44:23.507Z] [filter] deduped 25 → 24 (spam/history removed)
[2026-10-28T19:44:23.699Z] [enrich] techcrunch.com 109 → 1010 chars
[2026-10-28T19:44:24.379Z] [enrich] theverge.com 61 → 962 chars
[2026-10-28T19:44:24.385Z] [enrich] techcrunch.com 94 → 995 chars
[2026-10-28T19:44:24.400Z] [enrich] theverge.com 80 → 981 chars
[2026-10-28T19:44:25.983Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-28T19:44:26.446Z] [enrich] arstechnica.com 102 → 1003 chars
[2026-10-28T19:44:26.676Z] [enrich] arstechnica.com 108 → 1009 chars
[2026-10-28T19:44:26.929Z] [enrich] arstechnica.com 87 → 988 chars
[2026-10-28T19:44:26.929Z] Formatting 20 event candidates into the scan table.
[2026-10-28T19:53:44.093Z] [tracker] 6 deadlines tracked
[2026-10-28T19:53:44.094Z] [metrics] events candidates=20 picked=https://paypalaihackathon.devpost.com/ score=? domains=techcrunch.com,arstechnica.com,arstechnica.com,theverge.com,techcrunch.com,arstechnica.com,theverge.com,theverge.com
[2026-10-28T19:53:44.405Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
