---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-78481a87
created: 2026-11-14T07:13:09.308Z
jobId: 78481a87-0147-49a8-860f-3d39df4d2b1c
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-11-14T07:00:05.864Z
finishedAt: 2026-11-14T07:13:09.307Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-11-14T07:00:05.864Z
- **Finished:** 2026-11-14T07:13:09.307Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (8.1s)
2. ✓ Dedupe + rank — `pipeline` (84.7s)
3. ✓ Build weekend card — `pipeline` (782.8s)
4. ✓ Post to Telegram — `pipeline` (783.4s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-11-14
2-sentence factual summary: Zugwise presents a method to improve the accuracy of digitizing handwritten chess scoresheets by considering the domain-specific rules, which can help catch illegal moves more effectively.
Enjoy your weekend, here's to new discoveries and insights!

<details><summary>Log</summary>

```
[2026-11-14T07:00:05.873Z] Weekend sweep: Africa + World queries in one pass.
[2026-11-14T07:00:13.713Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-14T07:00:14.010Z] [weekend] web search gathered 15 candidates (quality-filtered).
[2026-11-14T07:00:14.046Z] [history] 147 URLs posted in last 7d
[2026-11-14T07:00:15.037Z] [enrich] arxiv.org 113 → 1014 chars
[2026-11-14T07:00:15.037Z] [enrich] arxiv.org 88 → 989 chars
[2026-11-14T07:00:18.164Z] [enrich] arxiv.org 97 → 998 chars
[2026-11-14T07:00:18.165Z] [enrich] arxiv.org 113 → 1014 chars
[2026-11-14T07:00:18.168Z] [enrich] arxiv.org 89 → 990 chars
[2026-11-14T07:00:18.169Z] [enrich] arxiv.org 99 → 1000 chars
[2026-11-14T07:01:30.560Z] [quality] scored 12 candidates — top: #1:8 Focuses on a specific and relevant AI ap | #6:6 Introduces a new platform for benchmarki | #5:5 Focuses on improving the robustness of a
[2026-11-14T07:01:30.560Z] Picked 3 stories for the weekend card.
[2026-11-14T07:13:08.630Z] [metrics] weekend candidates=23 picked=https://arxiv.org/abs/2611.14544 score=8 domains=arxiv.org,arxiv.org,arxiv.org,en.wikipedia.org,ontheworldmap.com,newzimbabwe.com,en.wikipedia.org,zimbabwetourism.net
[2026-11-14T07:13:09.307Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
