---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-183c774c
created: 2026-10-28T20:10:26.699Z
jobId: 183c774c-6ca8-447b-81de-576875b796bc
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-28T19:16:53.077Z
finishedAt: 2026-10-28T20:10:26.699Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-28T19:16:53.077Z
- **Finished:** 2026-10-28T20:10:26.699Z
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
1. ✓ Sweep event sources — `pipeline` (5.3s)
2. ✓ Dedupe + enrich — `pipeline` (5.3s)
3. ✓ Build events table — `pipeline` (538.4s)
4. ✓ Post to Telegram — `pipeline` (539.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-28

⭐ TOP PICK: Qloo Agentic Hackathon — win $25,000 in prizes, compete with 2733 participants, and showcase your machine learning/AI skills | https://qloo.devpost.com/

💻 Qloo Agentic Hackathon

6 free · 4 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-28T19:16:53.078Z] Queued — 7 tasks ahead (cap 2 running at once).
[2026-10-28T20:01:27.392Z] Started after 2674s in the task queue.
[2026-10-28T20:01:27.392Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-28T20:01:27.392Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-28T20:01:32.351Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-10-28T20:01:32.652Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-28T20:01:32.674Z] [history] 97 URLs posted in last 7d
[2026-10-28T20:01:32.674Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-10-28T20:01:32.674Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-10-28T20:01:32.679Z] [filter] deduped 25 → 23 (spam/history removed)
[2026-10-28T20:01:33.131Z] [enrich] techcrunch.com 94 → 995 chars
[2026-10-28T20:01:33.281Z] [enrich] techcrunch.com 109 → 1010 chars
[2026-10-28T20:01:33.536Z] [enrich] theverge.com 61 → 962 chars
[2026-10-28T20:01:33.559Z] [enrich] theverge.com 80 → 981 chars
[2026-10-28T20:01:33.869Z] [enrich] arstechnica.com 108 → 1009 chars
[2026-10-28T20:01:34.284Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-28T20:01:34.852Z] [enrich] arstechnica.com 102 → 1003 chars
[2026-10-28T20:01:35.049Z] [enrich] arstechnica.com 87 → 988 chars
[2026-10-28T20:01:35.050Z] Formatting 20 event candidates into the scan table.
[2026-10-28T20:10:25.754Z] [tracker] 7 deadlines tracked
[2026-10-28T20:10:25.756Z] [metrics] events candidates=20 picked=https://qloo.devpost.com/ score=? domains=techcrunch.com,arstechnica.com,arstechnica.com,theverge.com,techcrunch.com,arstechnica.com,theverge.com,theverge.com
[2026-10-28T20:10:26.699Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
