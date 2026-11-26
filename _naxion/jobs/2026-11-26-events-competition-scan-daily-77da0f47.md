---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-77da0f47
created: 2026-11-26T05:32:22.722Z
jobId: 77da0f47-fbe2-4e26-8009-5e931488980a
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-26T05:30:17.311Z
finishedAt: 2026-11-26T05:32:22.721Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-26T05:30:17.311Z
- **Finished:** 2026-11-26T05:32:22.721Z
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
1. ✓ Sweep event sources — `pipeline` (4.8s)
2. ✓ Dedupe + enrich — `pipeline` (4.9s)
3. ✓ Build events table — `pipeline` (124.5s)
4. ✓ Post to Telegram — `pipeline` (125.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-26

⭐ TOP PICK: GDG Harare Devfest Conference — Zimbabwe's premier community dev day covering ML, game dev, Angular & business; date TBA but follow GDG Harare for announcements | https://www.facebook.com/gdghararezw/

📅 EVENTS & COMPETITION SCAN — 2026-11-26
GDG Harare Devfest Conference — Zimbabwe's premier community dev day covering ML, game dev, Angular & business; date TBA but follow GDG Harare for announcements | https://www.facebook.com/gdghararezw/

🎪 GDG Harare Devfest Conference
📅 TBA | 📍 Harare, Zimbabwe | Free
🏆 — | ⏰ TBA
👥 Who: developers, students, tech enthusiasts | 🔗 https://www.facebook.com/gdghararezw/
💡 Why attend: connect with Zimbabwe's Google developer community and learn ML, game dev, Angular & business in one day

🌍 Devpost AI Hackathons Platform
📅 TBA (ongoing listings) | 📍 Remote | Free
🏆 Varies by hackathon (cash, prizes, exposure) | ⏰ TBA (varies by hackathon)
👥 Who: AI developers, builders, researchers | 🔗 https://devpost.com/c/artificial-intelligence
💡 Why attend: single hub to discover and join live AI hackathons with prizes from top AI companies

2 free · 0 paid · 1 remote global

2 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-26T05:30:17.459Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-26T05:30:17.460Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-26T05:30:21.002Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-26T05:30:22.220Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-26T05:30:22.313Z] [history] 189 URLs posted in last 7d
[2026-11-26T05:30:22.314Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-26T05:30:22.314Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-11-26T05:30:22.326Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-11-26T05:30:22.618Z] [enrich] arxiv.org 154 → 1055 chars
[2026-11-26T05:30:23.080Z] [enrich] arxiv.org 127 → 1028 chars
[2026-11-26T05:30:31.283Z] [enrich] arxiv.org 84 → 985 chars
[2026-11-26T05:30:31.300Z] [enrich] arxiv.org 108 → 1009 chars
[2026-11-26T05:30:31.314Z] [enrich] arxiv.org 139 → 1040 chars
[2026-11-26T05:30:31.315Z] [enrich] arxiv.org 108 → 1009 chars
[2026-11-26T05:30:31.315Z] [enrich] arxiv.org 93 → 994 chars
[2026-11-26T05:30:31.405Z] [enrich] huggingface.co 109 → 1010 chars
[2026-11-26T05:30:31.405Z] Formatting 20 event candidates into the scan table.
[2026-11-26T05:32:21.979Z] [tracker] 7 deadlines tracked
[2026-11-26T05:32:21.989Z] [metrics] events candidates=20 picked=https://www.facebook.com/gdghararezw/ score=? domains=arxiv.org,arxiv.org,arxiv.org,huggingface.co,arxiv.org,arxiv.org,arxiv.org,arxiv.org
[2026-11-26T05:32:22.721Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
