---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-3baa575c
created: 2026-10-28T19:29:06.024Z
jobId: 3baa575c-ba7d-4cfc-9845-08e0be40a8de
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-28T19:11:50.491Z
finishedAt: 2026-10-28T19:29:06.024Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-28T19:11:50.491Z
- **Finished:** 2026-10-28T19:29:06.024Z
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
1. ✓ Sweep event sources — `pipeline` (13.0s)
2. ✓ Dedupe + enrich — `pipeline` (13.1s)
3. ✓ Build events table — `pipeline` (728.6s)
4. ✓ Post to Telegram — `pipeline` (729.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-28

⭐ TOP PICK: Build With AI: Basics — learn AI best practices by creating a solid proof-of-concept for your dream project, with $25,000 in prizes | https://learn-ai-basics.devpost.com/

💻 Build With AI: Basics

7 free · 3 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-28T19:11:50.497Z] Queued — 0 tasks ahead (cap 2 running at once).
[2026-10-28T19:16:56.708Z] Started after 306s in the task queue.
[2026-10-28T19:16:56.709Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-28T19:16:56.710Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-28T19:17:02.240Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-28T19:17:09.750Z] [events] web search gathered 17 candidates (quality-filtered).
[2026-10-28T19:17:09.813Z] [history] 91 URLs posted in last 7d
[2026-10-28T19:17:10.523Z] [enrich] techcrunch.com 116 → 1017 chars
[2026-10-28T19:17:10.541Z] [enrich] techcrunch.com 94 → 995 chars
[2026-10-28T19:17:10.788Z] [enrich] aws.amazon.com 100 → 1001 chars
[2026-10-28T19:17:10.866Z] [enrich] theverge.com 73 → 974 chars
[2026-10-28T19:17:10.868Z] [enrich] theverge.com 80 → 981 chars
[2026-10-28T19:17:12.629Z] [enrich] arstechnica.com 114 → 1015 chars
[2026-10-28T19:17:13.112Z] [enrich] wired.com 121 → 1022 chars
[2026-10-28T19:17:14.597Z] [enrich] arstechnica.com 87 → 988 chars
[2026-10-28T19:17:14.598Z] Formatting 20 event candidates into the scan table.
[2026-10-28T19:29:05.296Z] [tracker] 5 deadlines tracked
[2026-10-28T19:29:05.299Z] [metrics] events candidates=20 picked=https://learn-ai-basics.devpost.com/ score=? domains=wired.com,techcrunch.com,arstechnica.com,aws.amazon.com,techcrunch.com,arstechnica.com,theverge.com,theverge.com
[2026-10-28T19:29:06.023Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
