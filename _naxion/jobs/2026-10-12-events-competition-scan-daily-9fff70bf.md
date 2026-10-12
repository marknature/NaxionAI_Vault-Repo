---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-9fff70bf
created: 2026-10-12T05:30:33.495Z
jobId: 9fff70bf-5c0a-4957-a5f1-12730f350784
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-12T05:30:15.578Z
finishedAt: 2026-10-12T05:30:33.494Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-12T05:30:15.578Z
- **Finished:** 2026-10-12T05:30:33.494Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (6.2s)
2. ✓ Dedupe + enrich — `pipeline` (6.2s)
3. ✓ Build events table — `pipeline` (17.0s)
4. ✓ Post to Telegram — `pipeline` (17.9s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-12

⭐ TOP PICK: Agents for Humans Hackathon — Build AI agents using Strands SDK to automate repetitive tasks | https://agentsforhumans.devpost.com/

🌍 Agents for Humans Hackathon

3 free · 0 paid · 3 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-12T05:30:15.584Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-12T05:30:15.584Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-12T05:30:20.349Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-12T05:30:21.751Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-12T05:30:21.762Z] [history] 27 URLs posted in last 7d
[2026-10-12T05:30:22.189Z] [enrich] arxiv.org 170 → 1071 chars
[2026-10-12T05:30:22.448Z] [enrich] arxiv.org 110 → 1011 chars
[2026-10-12T05:30:26.294Z] [enrich] arxiv.org 92 → 993 chars
[2026-10-12T05:30:26.296Z] [enrich] arxiv.org 100 → 1001 chars
[2026-10-12T05:30:26.298Z] [enrich] arxiv.org 115 → 1016 chars
[2026-10-12T05:30:26.300Z] [enrich] arxiv.org 167 → 1068 chars
[2026-10-12T05:30:26.307Z] [enrich] arxiv.org 101 → 1002 chars
[2026-10-12T05:30:26.307Z] [enrich] arxiv.org 129 → 1030 chars
[2026-10-12T05:30:26.308Z] Formatting 20 event candidates into the scan table.
[2026-10-12T05:30:32.587Z] [tracker] 2 deadlines tracked
[2026-10-12T05:30:32.588Z] [metrics] events candidates=20 picked=https://agentsforhumans.devpost.com/ score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-10-12T05:30:33.494Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
