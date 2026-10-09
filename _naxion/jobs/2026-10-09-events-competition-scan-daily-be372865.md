---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-be372865
created: 2026-10-09T05:30:36.874Z
jobId: be372865-591e-4766-b3d3-73e07708ea31
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-09T05:30:18.211Z
finishedAt: 2026-10-09T05:30:36.873Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-09T05:30:18.211Z
- **Finished:** 2026-10-09T05:30:36.873Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (7.3s)
2. ✓ Dedupe + enrich — `pipeline` (7.4s)
3. ✓ Build events table — `pipeline` (17.9s)
4. ✓ Post to Telegram — `pipeline` (18.7s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-09

⭐ TOP PICK: 2026 Hackathon – ML & AI for Zimbabwe's Banking Sector — High-stakes focus on financial inclusion in the local banking sector | https://opportunities.dsr.co.zw/

💻 2026 Hackathon – Machine Learning and Artificial Intelligence for Zimbabwe's Banking Sector and Financial Inclusion

5 free · 1 paid · 0 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-09T05:30:18.215Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-09T05:30:18.215Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-09T05:30:23.512Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-09T05:30:25.559Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-09T05:30:25.564Z] [history] 17 URLs posted in last 7d
[2026-10-09T05:30:25.565Z] [history] skip already-posted dev.events
[2026-10-09T05:30:25.565Z] [history] skip already-posted newspace.spaceinafrica.com
[2026-10-09T05:30:25.565Z] [history] skip already-posted africatechfestival.com
[2026-10-09T05:30:25.565Z] [history] skip already-posted engineeringforchange.org
[2026-10-09T05:30:25.565Z] [history] skip already-posted startupmaphub.com
[2026-10-09T05:30:25.568Z] [filter] deduped 23 → 18 (spam/history removed)
[2026-10-09T05:30:25.967Z] [enrich] arxiv.org 140 → 1041 chars
[2026-10-09T05:30:26.198Z] [enrich] arxiv.org 167 → 1068 chars
[2026-10-09T05:30:30.925Z] [enrich] arxiv.org 98 → 999 chars
[2026-10-09T05:30:30.929Z] [enrich] arxiv.org 117 → 1018 chars
[2026-10-09T05:30:30.930Z] [enrich] arxiv.org 87 → 988 chars
[2026-10-09T05:30:30.932Z] [enrich] arxiv.org 130 → 1031 chars
[2026-10-09T05:30:30.932Z] [enrich] arxiv.org 134 → 1035 chars
[2026-10-09T05:30:30.933Z] [enrich] arxiv.org 89 → 990 chars
[2026-10-09T05:30:30.933Z] Formatting 18 event candidates into the scan table.
[2026-10-09T05:30:36.121Z] [metrics] events candidates=18 picked=https://arxiv.org/abs/2610.10629 score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-10-09T05:30:36.873Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
