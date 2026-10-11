---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-13dea984
created: 2026-10-11T05:30:51.307Z
jobId: 13dea984-4373-4f28-8a6f-4bfef1fbe8f7
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-11T05:30:17.672Z
finishedAt: 2026-10-11T05:30:51.306Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-11T05:30:17.672Z
- **Finished:** 2026-10-11T05:30:51.306Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (9.7s)
2. ✓ Dedupe + enrich — `pipeline` (9.8s)
3. ✓ Build events table — `pipeline` (33.3s)
4. ✓ Post to Telegram — `pipeline` (33.6s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-11

⭐ TOP PICK: TechCrunch Disrupt 2026 — High-visibility networking and startup exposure starting in 2 days | https://techcrunch.com/

🎪 TechCrunch Disrupt 2026

2 free · 1 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-11T05:30:17.688Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-11T05:30:17.688Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-11T05:30:24.098Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-11T05:30:27.430Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-11T05:30:27.445Z] [history] 25 URLs posted in last 7d
[2026-10-11T05:30:27.726Z] [enrich] theverge.com 96 → 997 chars
[2026-10-11T05:30:27.729Z] [enrich] theverge.com 89 → 990 chars
[2026-10-11T05:30:27.736Z] [enrich] theverge.com 92 → 993 chars
[2026-10-11T05:30:28.050Z] [enrich] ventureburn.com 129 → 533 chars
[2026-10-11T05:30:28.260Z] [enrich] techcrunch.com 95 → 996 chars
[2026-10-11T05:30:28.513Z] [enrich] simonwillison.net 69 → 970 chars
[2026-10-11T05:30:28.530Z] [enrich] simonwillison.net 76 → 977 chars
[2026-10-11T05:30:44.577Z] [enrich] techcrunch.com 118 → 1019 chars
[2026-10-11T05:30:44.577Z] Formatting 20 event candidates into the scan table.
[2026-10-11T05:30:51.026Z] [tracker] 1 deadlines tracked
[2026-10-11T05:30:51.028Z] [metrics] events candidates=20 picked=https://techcrunch.com/ score=? domains=ventureburn.com,techcrunch.com,theverge.com,techcrunch.com,theverge.com,theverge.com,simonwillison.net,simonwillison.net
[2026-10-11T05:30:51.305Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
