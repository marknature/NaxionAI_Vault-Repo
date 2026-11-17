---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-40d27e15
created: 2026-10-29T19:20:18.824Z
jobId: 40d27e15-4878-4561-b642-2a8a97d15aaf
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-29T18:54:08.349Z
finishedAt: 2026-10-29T19:20:18.823Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-29T18:54:08.349Z
- **Finished:** 2026-10-29T19:20:18.823Z
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
1. ✓ Sweep event sources — `pipeline` (20.0s)
2. ✓ Dedupe + enrich — `pipeline` (20.0s)
3. ✓ Build events table — `pipeline` (949.3s)
4. ✓ Post to Telegram — `pipeline` (949.7s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-29

⭐ TOP PICK: Qloo Agentic Hackathon — win $25,000 in prizes, don't miss the last day to participate | https://qloo.devpost.com/?ref_feature=challenge&ref_medium=discover

💻 Qloo Agentic Hackathon

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-29T18:54:08.349Z] Queued — 1 task ahead (cap 2 running at once).
[2026-10-29T19:04:29.129Z] Started after 621s in the task queue.
[2026-10-29T19:04:29.129Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-29T19:04:29.129Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-29T19:04:41.765Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-29T19:04:49.115Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-10-29T19:04:49.154Z] [history] 99 URLs posted in last 7d
[2026-10-29T19:04:49.155Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-10-29T19:04:49.155Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-10-29T19:04:49.162Z] [filter] deduped 25 → 23 (spam/history removed)
[2026-10-29T19:04:49.898Z] [enrich] techcrunch.com 90 → 991 chars
[2026-10-29T19:04:50.284Z] [enrich] theverge.com 97 → 998 chars
[2026-10-29T19:04:50.417Z] [enrich] theverge.com 81 → 982 chars
[2026-10-29T19:04:50.485Z] [enrich] theverge.com 95 → 996 chars
[2026-10-29T19:04:50.624Z] [enrich] ventureburn.com 104 → 727 chars
[2026-10-29T19:04:51.336Z] [enrich] wired.com 108 → 1009 chars
[2026-10-29T19:04:52.902Z] [enrich] arstechnica.com 76 → 977 chars
[2026-10-29T19:04:52.985Z] [enrich] arstechnica.com 109 → 1010 chars
[2026-10-29T19:04:52.985Z] Formatting 20 event candidates into the scan table.
[2026-10-29T19:20:18.404Z] [tracker] 7 deadlines tracked
[2026-10-29T19:20:18.409Z] [metrics] events candidates=20 picked=https://qloo.devpost.com/?ref_feature=challenge&ref_medium=discover score=? domains=arstechnica.com,wired.com,ventureburn.com,theverge.com,theverge.com,techcrunch.com,theverge.com,arstechnica.com
[2026-10-29T19:20:18.823Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
