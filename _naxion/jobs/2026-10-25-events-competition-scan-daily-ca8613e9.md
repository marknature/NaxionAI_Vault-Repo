---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-ca8613e9
created: 2026-10-25T05:36:49.103Z
jobId: ca8613e9-1a70-40f7-82e6-7a89d3b4a79c
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-25T05:30:22.640Z
finishedAt: 2026-10-25T05:36:49.102Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-25T05:30:22.640Z
- **Finished:** 2026-10-25T05:36:49.102Z
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
1. ✓ Sweep event sources — `pipeline` (43.7s)
2. ✓ Dedupe + enrich — `pipeline` (43.7s)
3. ✓ Build events table — `pipeline` (385.7s)
4. ✓ Post to Telegram — `pipeline` (386.5s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-25

⭐ TOP PICK: The Innovation Challenge — win funding, mentorship, and international exposure for your startup idea | https://www.instagram.com/p/DTuk86NmoiP/

💻 IEB TechWays AI Hackathon 2026

7 free · 3 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-25T05:30:22.644Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-25T05:30:22.644Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-25T05:31:06.321Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-25T05:31:06.338Z] [history] 76 URLs posted in last 7d
[2026-10-25T05:31:06.338Z] [history] skip already-posted africatechfestival.com
[2026-10-25T05:31:06.339Z] [filter] deduped 15 → 14 (spam/history removed)
[2026-10-25T05:31:07.461Z] [enrich] facebook.com 144 → 282 chars
[2026-10-25T05:31:07.513Z] [enrich] play.google.com 145 → 1046 chars
[2026-10-25T05:31:07.626Z] [enrich] play.google.com 192 → 1093 chars
[2026-10-25T05:31:07.938Z] [enrich] facebook.com 159 → 297 chars
[2026-10-25T05:31:08.528Z] [enrich] dev.events 155 → 573 chars
[2026-10-25T05:31:09.613Z] [enrich] opportunities.dsr.co.zw 157 → 1058 chars
[2026-10-25T05:31:11.010Z] [enrich] dev.events 148 → 1049 chars
[2026-10-25T05:31:12.689Z] [enrich] techways.online 302 → 1100 chars
[2026-10-25T05:31:12.690Z] Formatting 14 event candidates into the scan table.
[2026-10-25T05:36:48.324Z] [tracker] 5 deadlines tracked
[2026-10-25T05:36:48.326Z] [metrics] events candidates=14 picked=https://www.instagram.com/p/DTuk86NmoiP/ score=? domains=techways.online,play.google.com,facebook.com,opportunities.dsr.co.zw,dev.events,dev.events,play.google.com,facebook.com
[2026-10-25T05:36:49.102Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
