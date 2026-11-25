---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-61522800
created: 2026-11-25T05:32:13.665Z
jobId: 61522800-4a09-4e96-8e00-40fef85fc72f
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-11-25T05:30:22.388Z
finishedAt: 2026-11-25T05:32:13.665Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-11-25T05:30:22.388Z
- **Finished:** 2026-11-25T05:32:13.665Z
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
1. ✓ Sweep event sources — `pipeline` (8.9s)
2. ✓ Dedupe + enrich — `pipeline` (9.0s)
3. ✓ Build events table — `pipeline` (110.3s)
4. ✓ Post to Telegram — `pipeline` (111.3s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-11-25

⭐ TOP PICK: HackWithAditya — ₹500k prize, deadline today, global AI hackathon | https://hackwithaditya.devpost.com/

📅 EVENTS & COMPETITION SCAN — 2026-11-25
HackWithAditya — ₹500k prize, deadline today, global AI hackathon | https://hackwithaditya.devpost.com/

🌍 HackWithAditya
📅 Nov 25 (0 days left) – submission deadline | 📍 Remote | Free
🏆 ₹500,000 | ⏰ Nov 25 (0 days left)
👥 Who: AI developers, builders | 🔗 https://hackwithaditya.devpost.com/
💡 Why attend: Win ₹500k cash building AI projects, global exposure on Devpost

1 free · 0 paid · 1 remote global
HackWithAditya | 2026-11-25 | https://hackwithaditya.devpost.com/

1 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-11-25T05:30:22.411Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-11-25T05:30:22.411Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-11-25T05:30:27.641Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-25T05:30:31.296Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-11-25T05:30:31.396Z] [history] 186 URLs posted in last 7d
[2026-11-25T05:30:31.398Z] [history] skip already-posted paypalaihackathon.devpost.com
[2026-11-25T05:30:31.398Z] [history] skip already-posted learn-ai-basics.devpost.com
[2026-11-25T05:30:31.408Z] [filter] deduped 23 → 21 (spam/history removed)
[2026-11-25T05:30:31.649Z] [enrich] simonwillison.net 74 → 975 chars
[2026-11-25T05:30:31.678Z] [enrich] theverge.com 112 → 1013 chars
[2026-11-25T05:30:31.683Z] [enrich] techcrunch.com 111 → 1012 chars
[2026-11-25T05:30:31.713Z] [enrich] theverge.com 86 → 987 chars
[2026-11-25T05:30:31.753Z] [enrich] theverge.com 61 → 962 chars
[2026-11-25T05:30:32.877Z] [enrich] wired.com 79 → 980 chars
[2026-11-25T05:30:44.316Z] [enrich] arstechnica.com 97 → 998 chars
[2026-11-25T05:30:44.326Z] [enrich] arstechnica.com 95 → 996 chars
[2026-11-25T05:30:44.326Z] Formatting 20 event candidates into the scan table.
[2026-11-25T05:32:12.724Z] [tracker] 7 deadlines tracked
[2026-11-25T05:32:12.771Z] [metrics] events candidates=20 picked=https://hackwithaditya.devpost.com/ score=? domains=theverge.com,techcrunch.com,arstechnica.com,arstechnica.com,theverge.com,wired.com,simonwillison.net,theverge.com
[2026-11-25T05:32:13.665Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
