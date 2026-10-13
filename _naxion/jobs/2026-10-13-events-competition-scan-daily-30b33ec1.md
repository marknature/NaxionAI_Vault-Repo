---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-30b33ec1
created: 2026-10-13T05:30:29.002Z
jobId: 30b33ec1-ce61-4364-b798-0f24a9afe4da
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-13T05:30:10.988Z
finishedAt: 2026-10-13T05:30:29.001Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-13T05:30:10.988Z
- **Finished:** 2026-10-13T05:30:29.001Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (6.1s)
2. ✓ Dedupe + enrich — `pipeline` (6.1s)
3. ✓ Build events table — `pipeline` (17.0s)
4. ✓ Post to Telegram — `pipeline` (18.0s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-13

⭐ TOP PICK: MLAI Hackathon 2026 — High-visibility AI application challenge with a tight 3-day window | https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 MLAI Hackathon 2026

1 free · 1 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-13T05:30:10.994Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-13T05:30:10.994Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-13T05:30:15.738Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-13T05:30:17.125Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-13T05:30:17.128Z] [history] 31 URLs posted in last 7d
[2026-10-13T05:30:17.128Z] [history] skip already-posted agentsforhumans.devpost.com
[2026-10-13T05:30:17.131Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-13T05:30:17.414Z] [enrich] blogs.nvidia.com 114 → 1015 chars
[2026-10-13T05:30:17.572Z] [enrich] arxiv.org 170 → 1071 chars
[2026-10-13T05:30:22.222Z] [enrich] arxiv.org 101 → 1002 chars
[2026-10-13T05:30:22.223Z] [enrich] arxiv.org 100 → 1001 chars
[2026-10-13T05:30:22.459Z] [enrich] arxiv.org 129 → 1030 chars
[2026-10-13T05:30:22.459Z] [enrich] arxiv.org 115 → 1016 chars
[2026-10-13T05:30:22.608Z] [enrich] arxiv.org 167 → 1068 chars
[2026-10-13T05:30:22.766Z] [enrich] arxiv.org 92 → 993 chars
[2026-10-13T05:30:22.766Z] Formatting 20 event candidates into the scan table.
[2026-10-13T05:30:27.980Z] [tracker] 4 deadlines tracked
[2026-10-13T05:30:27.981Z] [metrics] events candidates=20 picked=https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=arxiv.org,arxiv.org,arxiv.org,arxiv.org,blogs.nvidia.com,arxiv.org,arxiv.org,arxiv.org
[2026-10-13T05:30:29.001Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
