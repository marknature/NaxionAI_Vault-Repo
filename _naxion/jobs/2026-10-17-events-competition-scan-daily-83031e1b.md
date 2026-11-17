---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-83031e1b
created: 2026-10-17T06:17:06.842Z
jobId: 83031e1b-0018-4427-8e95-610dc902eec0
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-17T06:12:59.654Z
finishedAt: 2026-10-17T06:17:06.842Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-17T06:12:59.654Z
- **Finished:** 2026-10-17T06:17:06.842Z
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
3. ✓ Build events table — `pipeline` (98.8s)
4. ✓ Post to Telegram — `pipeline` (99.5s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-17

⭐ TOP PICK: Transforming Enterprise Through AI lablab.ai Hackathon — win exposure and skills (TBA prize, TBA deadline) | https://lablab.ai/ai-hackathons/techex-intelligent-enterprise-solutions-hackathon

📅 EVENTS & COMPETITION SCAN — 2026-10-17
Transforming Enterprise Through AI lablab.ai Hackathon — win exposure and skills (TBA prize, TBA deadline) | https://lablab.ai/ai-hackathons/techex-intelligent-enterprise-solutions-hackathon

🎪 GDG Harare Pre DevFest Workshop
📅 TBA | 📍 Harare, Zimbabwe | Free
🏆 TBA | ⏰ TBA
👥 Who: developers, tech enthusiasts | 🔗 https://gdg.community.dev/gdg-harare/
💡 Why attend: hands-on learning with Google Developer Experts to boost your Google Cloud skills.

💻 Transforming Enterprise Through AI lablab.ai Hackathon
📅 TBA | 📍 Remote (lablab.ai platform & Discord) | Free
🏆 TBA | ⏰ TBA
👥 Who: AI builders, developers | 🔗 https://lablab.ai/ai-hackathons/techex-intelligent-enterprise-solutions-hackathon
💡 Why attend: collaborate on real‑world AI challenges for enterprises and gain visibility in the global AI builder community.

2 free · 0 paid · 1 remote global

2 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-17T06:12:59.655Z] Queued — 0 tasks ahead (cap 2 running at once).
[2026-10-17T06:15:27.297Z] Started after 148s in the task queue.
[2026-10-17T06:15:27.297Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-17T06:15:27.297Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-17T06:15:29.302Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-17T06:15:32.555Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-17T06:15:32.561Z] [history] 32 URLs posted in last 7d
[2026-10-17T06:15:32.561Z] [history] skip already-posted lablab.ai
[2026-10-17T06:15:32.566Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-17T06:16:09.851Z] [enrich] theverge.com 111 → 1012 chars
[2026-10-17T06:16:09.886Z] [enrich] theverge.com 107 → 1008 chars
[2026-10-17T06:16:09.949Z] [enrich] techcrunch.com 81 → 982 chars
[2026-10-17T06:16:09.956Z] [enrich] simonwillison.net 85 → 986 chars
[2026-10-17T06:16:10.026Z] [enrich] arstechnica.com 91 → 992 chars
[2026-10-17T06:16:10.101Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-17T06:16:10.266Z] [enrich] theverge.com 58 → 959 chars
[2026-10-17T06:16:10.516Z] [enrich] aws.amazon.com 139 → 1040 chars
[2026-10-17T06:16:10.516Z] Formatting 20 event candidates into the scan table.
[2026-10-17T06:17:06.123Z] [tracker] 7 deadlines tracked
[2026-10-17T06:17:06.124Z] [metrics] events candidates=20 picked=https://lablab.ai/ai-hackathons/techex-intelligent-enterprise-solutions-hackathon score=? domains=aws.amazon.com,theverge.com,theverge.com,theverge.com,arstechnica.com,simonwillison.net,techcrunch.com,theverge.com
[2026-10-17T06:17:06.841Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
