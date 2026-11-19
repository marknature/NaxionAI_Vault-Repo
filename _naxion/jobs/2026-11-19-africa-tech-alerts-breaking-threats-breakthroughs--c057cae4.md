---
type: job
title: Africa Tech Alerts — BREAKING (threats & breakthroughs)
slug: africa-tech-alerts-breaking-threats-breakthroughs--c057cae4
created: 2026-11-19T10:33:40.792Z
jobId: c057cae4-3c5e-49c9-8763-f566ec68cf77
status: succeeded
template: africa-tech-alerts
persona: naxie
personaName: Naxie
startedAt: 2026-11-19T10:30:05.252Z
finishedAt: 2026-11-19T10:33:40.792Z
---

# Africa Tech Alerts — BREAKING (threats & breakthroughs)

- **Status:** succeeded
- **Template:** africa-tech-alerts
- **Started:** 2026-11-19T10:30:05.252Z
- **Finished:** 2026-11-19T10:33:40.792Z
- **Title:** Africa Tech Alerts — BREAKING (threats & breakthroughs)

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep threats + breakthroughs — `pipeline` (95.2s)
2. ✓ Dedupe + enrich — `pipeline` (95.2s)
3. ✓ Quality rank — `pipeline` (167.7s)
4. ✓ Build alerts card — `pipeline` (214.6s)
5. ✓ Post to Telegram — `pipeline` (215.5s)

## Answer
⚡ AFRICA TECH ALERTS — Daily

Ethiopian Airlines reports cyberattack a week after Air Botswana

Ethiopian Airlines has reported a cyberattack, following a similar incident at Air Botswana a week prior. Both airlines are part of the Ethiopian Airlines Group, which has faced multiple cybersecurity challenges in recent months.

Why it matters
This incident highlights the ongoing cybersecurity risks faced by airlines, particularly those operating in regions with less stringent regulatory frameworks, and underscores the importance of robust cybersecurity measures to protect critical infrastructure.

📰 Read more: https://techcabal.com/2026/11/18/ethiopian-airlines-reports-cyberattack/

#Africa #TechAlerts #AINews #Cybersecurity #Airlines #EthiopianAirlines

Source: RSS ≤48h + web search (threats + breakthroughs)
Story: **Ethiopian Airlines reports cyberattack a week after Air Botswana:** [TechCabal · 2026-11-18] Ethiopian Airlines reports cyberattack a week after Air Botswana — https://techcabal.com/2026/11/18/ethiopian-airlines-reports-cyberattack/

<details><summary>Log</summary>

```
[2026-11-19T10:30:05.264Z] Sweeping for dangerous or amazing tech in, around and to Africa.
[2026-11-19T10:30:05.265Z] [alerts] quality pipeline: RSS (≤48h) + threat/breakthrough search → dedupe → enrich → quality rank
[2026-11-19T10:30:11.809Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-11-19T10:31:40.423Z] [alerts] web search gathered 8 candidates (quality-filtered).
[2026-11-19T10:31:40.454Z] [history] 167 URLs posted in last 7d
[2026-11-19T10:31:40.454Z] [history] skip already-posted techinafrica.com
[2026-11-19T10:31:40.455Z] [history] skip already-posted openai.com
[2026-11-19T10:31:40.455Z] [history] skip already-posted ai.google
[2026-11-19T10:31:40.456Z] [filter] deduped 16 → 13 (spam/history removed)
[2026-11-19T10:31:41.514Z] [enrich] techinafrica.com 116 → 621 chars
[2026-11-19T10:31:43.110Z] [enrich] wired.com 90 → 991 chars
[2026-11-19T10:31:57.294Z] [enrich] techcabal.com 92 → 835 chars
[2026-11-19T10:31:57.294Z] [enrich] techcabal.com 92 → 835 chars
[2026-11-19T10:31:57.309Z] [enrich] techinafrica.com 158 → 433 chars
[2026-11-19T10:31:57.527Z] [enrich] iafrica.com 90 → 242 chars
[2026-11-19T10:32:52.965Z] [quality] scored 12 candidates — top: #1:10 African fintech focus with specific inve | #2:7 African tech event but not specific to f | #3:5 Local fintech news but not specific to A
[2026-11-19T10:32:52.965Z] Picked 12 fresh candidates (top score 10) — drafting the daily card.
[2026-11-19T10:33:39.832Z] [metrics] alerts candidates=12 picked=https://techcabal.com/2026/11/18/ethiopian-airlines-reports-cyberattack/ score=4 domains=techinafrica.com,techinafrica.com,techcabal.com,techcabal.com,iafrica.com,deepai.org,techcabal.com,wired.com
[2026-11-19T10:33:40.791Z] Posted Africa Tech Alerts to Telegram chat -1004307136262.
```
</details>
