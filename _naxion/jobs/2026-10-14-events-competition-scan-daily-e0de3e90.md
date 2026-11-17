---
type: job
title: Events & Competition Scan — daily
slug: events-competition-scan-daily-e0de3e90
created: 2026-10-14T05:30:37.754Z
jobId: e0de3e90-7f4a-47b1-ac57-45239cd170e0
status: succeeded
template: events-competition-scan
persona: naxie
personaName: Naxie
startedAt: 2026-10-14T05:30:09.833Z
finishedAt: 2026-10-14T05:30:37.753Z
---

# Events & Competition Scan — daily

- **Status:** succeeded
- **Template:** events-competition-scan
- **Started:** 2026-10-14T05:30:09.833Z
- **Finished:** 2026-10-14T05:30:37.753Z
- **Title:** Events & Competition Scan — daily

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep event sources — `pipeline` (5.3s)
2. ✓ Dedupe + enrich — `pipeline` (5.4s)
3. ✓ Build events table — `pipeline` (26.9s)
4. ✓ Post to Telegram — `pipeline` (27.9s)

## Answer
📅 EVENTS & COMPETITION SCAN — 2026-10-14

⭐ TOP PICK: MLAI Hackathon 2026 — High-visibility AI application challenge with a tight 2-day submission window | https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel

🌍 MLAI Hackathon 2026

1 free · 0 paid · 1 remote global

Source: web sweep (RSS ≤48h + event listings + hackathon hubs)

<details><summary>Log</summary>

```
[2026-10-14T05:30:09.847Z] Sweeping tech events, hackathons and competitions (ZW + SA + pan-African + global remote).
[2026-10-14T05:30:09.848Z] [events] pipeline: RSS (≤48h) + events web search → dedupe → enrich
[2026-10-14T05:30:14.709Z] [events] web search gathered 15 candidates (quality-filtered).
[2026-10-14T05:30:15.193Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-14T05:30:15.208Z] [history] 33 URLs posted in last 7d
[2026-10-14T05:30:15.208Z] [history] skip already-posted agentsforhumans.devpost.com
[2026-10-14T05:30:15.218Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-10-14T05:30:22.195Z] [enrich] simonwillison.net 69 → 970 chars
[2026-10-14T05:30:22.260Z] [enrich] ventureburn.com 88 → 799 chars
[2026-10-14T05:30:22.284Z] [enrich] techcrunch.com 122 → 1023 chars
[2026-10-14T05:30:22.479Z] [enrich] techcrunch.com 103 → 1004 chars
[2026-10-14T05:30:22.498Z] [enrich] wired.com 114 → 1015 chars
[2026-10-14T05:30:22.601Z] [enrich] techcrunch.com 126 → 1027 chars
[2026-10-14T05:30:27.460Z] [enrich] deepmind.google 131 → 1032 chars
[2026-10-14T05:30:32.186Z] [enrich] arstechnica.com 103 → 1004 chars
[2026-10-14T05:30:32.186Z] Formatting 20 event candidates into the scan table.
[2026-10-14T05:30:36.737Z] [tracker] 4 deadlines tracked
[2026-10-14T05:30:36.740Z] [metrics] events candidates=20 picked=https://mlai-hackathon.devpost.com/?ref_content=online-hackathons&ref_feature=challenge&ref_medium=artificial-intelligence-channel score=? domains=deepmind.google,techcrunch.com,techcrunch.com,wired.com,techcrunch.com,arstechnica.com,ventureburn.com,simonwillison.net
[2026-10-14T05:30:37.752Z] Posted Events & Competition Scan to Telegram chat 8767926406.
```
</details>
