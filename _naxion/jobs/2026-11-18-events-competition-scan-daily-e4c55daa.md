---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-e4c55daa
created: 2026-11-18T05:35:28.656Z
jobId: e4c55daa-554c-4998-a205-e8e5fd7acc35
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-18T05:30:24.271Z
finishedAt: 2026-11-18T05:35:28.655Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-18T05:30:24.271Z
- **Finished:** 2026-11-18T05:35:28.655Z
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
1. ✓ Sweep event sources — `pipeline` (7.3s)
2. ✓ Dedupe + enrich — `pipeline` (7.5s)
3. ✓ Build events table — `pipeline` (303.6s)
4. ✓ Post to Telegram — `pipeline` (304.4s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-18

⭐ TOP PICK: ZIMSEC Regional Staff Registration - CAMC System | — | https://camc.zimsec.co.zw/Identity/Account/RegisterRegional

🏠 ZIMSEC Regional Staff Registration - CAMC System | 📅 2026-11-18 | 📍 https://camc.zimsec.co.zw/Identity/Account/RegisterRegional | 🏷️ 🌍

8 free · 2 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-18T05:30:24.282Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-18T05:30:24.282Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-18T05:30:30.452Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-18T05:30:31.599Z] [events] web search gathered 16 candidates (quality-filtered).
[2026-11-18T05:30:31.783Z] [history] 161 URLs posted in last 7d
[2026-11-18T05:30:31.783Z] [history] skip already-posted support.microsoft.com
[2026-11-18T05:30:31.794Z] [filter] deduped 24 → 23 (spam/history removed)
[2026-11-18T05:30:32.404Z] [enrich] arxiv.org 126 → 1027 chars
[2026-11-18T05:30:33.321Z] [enrich] wired.com 75 → 976 chars
[2026-11-18T05:30:36.966Z] [enrich] arxiv.org 102 → 1003 chars
[2026-11-18T05:30:36.967Z] [enrich] arxiv.org 95 → 996 chars
[2026-11-18T05:30:36.967Z] [enrich] arxiv.org 158 → 1059 chars
[2026-11-18T05:30:36.968Z] [enrich] arxiv.org 110 → 1011 chars
[2026-11-18T05:30:37.282Z] [enrich] support.microsoft.com 121 → 1022 chars
[2026-11-18T05:30:37.650Z] [enrich] support.microsoft.com 134 → 1035 chars
[2026-11-18T05:30:37.650Z] Formatting 20 event candidates into the scan table.
[2026-11-18T05:35:27.879Z] [tracker] 9 deadlines tracked
[2026-11-18T05:35:27.881Z] [metrics] events candidates=20 picked=https://camc.zimsec.co.zw/Identity/Account/RegisterRegional score=? domains=arxiv.org,support.microsoft.com,arxiv.org,support.microsoft.com,arxiv.org,arxiv.org,arxiv.org,wired.com
[2026-11-18T05:35:28.655Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
