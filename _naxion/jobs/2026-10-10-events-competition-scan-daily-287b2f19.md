---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-287b2f19
created: 2026-10-10T05:30:46.516Z
jobId: 287b2f19-0ea9-4106-8fdc-3ccb03ed5c16
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-10T05:30:24.101Z
finishedAt: 2026-10-10T05:30:46.515Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-10T05:30:24.101Z
- **Finished:** 2026-10-10T05:30:46.515Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (4.9s)
2. ✓ Dedupe + enrich — `pipeline` (4.9s)
3. ✓ Build events table — `pipeline` (21.6s)
4. ✓ Post to Telegram — `pipeline` (22.4s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-10

⭐ TOP PICK: AI Hackathon with Google DeepMind — High-tier technical collaboration with DeepMind engineers | https://gdg.community.dev/events/details/google-gdg-cape-town-presents-ai-hackathon-with-google-deepmind/

💻 DevFest Harare 2026

7 free · 0 paid · 0 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-10T05:30:24.125Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-10T05:30:24.125Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-10T05:30:28.803Z] [events] web search gathered 14 candidates (quality-filtered).
[2026-10-10T05:30:28.979Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-10T05:30:28.992Z] [history] 22 URLs posted in last 7d
[2026-10-10T05:30:28.993Z] [history] skip already-posted opportunities.dsr.co.zw
[2026-10-10T05:30:28.993Z] [history] skip already-posted dev.events
[2026-10-10T05:30:28.993Z] [history] skip already-posted newspace.spaceinafrica.com
[2026-10-10T05:30:28.993Z] [history] skip already-posted africatechfestival.com
[2026-10-10T05:30:28.993Z] [history] skip already-posted engineeringforchange.org
[2026-10-10T05:30:28.993Z] [history] skip already-posted startupmaphub.com
[2026-10-10T05:30:28.998Z] [filter] deduped 22 → 16 (spam/history removed)
[2026-10-10T05:30:29.098Z] [enrich] techcrunch.com 103 → 1004 chars
[2026-10-10T05:30:29.114Z] [enrich] theverge.com 60 → 961 chars
[2026-10-10T05:30:29.764Z] [enrich] techcrunch.com 155 → 1056 chars
[2026-10-10T05:30:29.932Z] [enrich] simonwillison.net 56 → 957 chars
[2026-10-10T05:30:29.981Z] [enrich] simonwillison.net 56 → 957 chars
[2026-10-10T05:30:40.463Z] [enrich] arstechnica.com 88 → 989 chars
[2026-10-10T05:30:40.522Z] [enrich] arstechnica.com 87 → 988 chars
[2026-10-10T05:30:40.553Z] [enrich] arstechnica.com 100 → 1001 chars
[2026-10-10T05:30:40.553Z] Formatting 16 event candidates into the scan table.
[2026-10-10T05:30:45.719Z] [metrics] events candidates=16 picked=https://techcrunch.com/2026/10/09/anthropic-cant-reliably-control-its-ai-agents-its-cutting-off-its-internal-evals-from-the-live-internet-instead/ score=? domains=techcrunch.com,techcrunch.com,arstechnica.com,arstechnica.com,arstechnica.com,theverge.com,simonwillison.net,simonwillison.net
[2026-10-10T05:30:46.515Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
