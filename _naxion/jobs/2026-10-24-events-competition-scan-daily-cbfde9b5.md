---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-cbfde9b5
created: 2026-10-24T05:38:01.805Z
jobId: cbfde9b5-a8f0-48e7-99bc-0743a8137ceb
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-24T05:30:26.858Z
finishedAt: 2026-10-24T05:38:01.805Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-24T05:30:26.858Z
- **Finished:** 2026-10-24T05:38:01.805Z
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
1. ✓ Sweep event sources — `pipeline` (7.9s)
2. ✓ Dedupe + enrich — `pipeline` (7.9s)
3. ✓ Build events table — `pipeline` (454.2s)
4. ✓ Post to Telegram — `pipeline` (454.9s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-24

⭐ TOP PICK: Google and Elba Hope Foundation Launch $1 Million AI Initiative for African Creators | URL: https://www.techinafrica.com/google-and-elba-hope-foundation-launch-1-million-ai-initiative-for-african-creators/ (prize/deadline hook) | $1 Million in prizes, deadline TBA

💻 UGREEN Hackathon 2026 on AI NAS

6 free · 4 paid · 2 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-24T05:30:26.862Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-24T05:30:26.862Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-24T05:30:31.139Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-24T05:30:34.644Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-24T05:30:34.799Z] [history] 70 URLs posted in last 7d
[2026-10-24T05:30:34.799Z] [history] skip already-posted lablab.ai
[2026-10-24T05:30:34.799Z] [history] skip already-posted gdg.community.dev
[2026-10-24T05:30:34.803Z] [filter] deduped 23 → 20 (spam/history removed)
[2026-10-24T05:30:34.964Z] [enrich] techcrunch.com 127 → 1028 chars
[2026-10-24T05:30:34.980Z] [enrich] techcrunch.com 116 → 1017 chars
[2026-10-24T05:30:35.282Z] [enrich] theverge.com 92 → 993 chars
[2026-10-24T05:30:35.283Z] [enrich] theverge.com 89 → 990 chars
[2026-10-24T05:30:35.709Z] [enrich] arstechnica.com 114 → 1015 chars
[2026-10-24T05:30:36.038Z] [enrich] devpost.com 471 → 1100 chars
[2026-10-24T05:30:36.511Z] [enrich] techinafrica.com 114 → 1015 chars
[2026-10-24T05:30:36.903Z] [enrich] arstechnica.com 104 → 1005 chars
[2026-10-24T05:30:36.903Z] Formatting 20 event candidates into the scan table.
[2026-10-24T05:38:01.070Z] [tracker] 6 deadlines tracked
[2026-10-24T05:38:01.073Z] [metrics] events candidates=20 picked=https://www.techinafrica.com/google-and-elba-hope-foundation-launch-1-million-ai-initiative-for-african-creators/ score=? domains=techcrunch.com,techcrunch.com,arstechnica.com,techinafrica.com,arstechnica.com,theverge.com,theverge.com,devpost.com
[2026-10-24T05:38:01.805Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
