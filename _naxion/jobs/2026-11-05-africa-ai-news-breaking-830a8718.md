---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-830a8718
created: 2026-11-05T08:00:22.837Z
jobId: 830a8718-85dc-43fa-bcdf-84b9129daae4
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-05T08:00:02.108Z
finishedAt: 2026-11-05T08:00:22.835Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-05T08:00:02.108Z
- **Finished:** 2026-11-05T08:00:22.835Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "chatId": "<existing>",
  "videoUrl": "<existing>"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (10.4s)
2. ✓ Dedupe + enrich — `pipeline` (10.5s)
3. ✓ Quality rank — `pipeline` (17.4s)
4. ✓ Build news card — `pipeline` (19.5s)
5. ✓ Post to Telegram — `pipeline` (20.7s)

## Answer
🚨 BREAKING NEWS — Africa AI 🚨

South Africa Withdraws AI Policy After Hallucinated Citations

South Africa has pulled its draft AI policy after it was discovered that AI hallucinations fabricated at least six of the 67 academic citations used. The ambitious policy had proposed five new oversight bodies, including a National AI Commission and an AI Insurance Superfund to compensate citizens harmed by the technology. There is currently no timeline for a revised draft, leaving the country's digital economy in regulatory limbo.

Why it matters for Africa
This incident serves as a stark warning about the risks of relying on AI for governance and policy drafting. It highlights the critical need for human oversight and verification to ensure regulatory frameworks are grounded in factual evidence.

📰 Read more: https://www.cnbcafrica.com/2026/south-africa-pulls-ai-policy-after-hallucinated-citations-expose-drafting-scandal

#AI #Africa #AINews #SouthAfrica #Governance #TechPolicy

Source: web + innovation leads (RSS ≤48h + web + leads)
Story: **South Africa Withdraws AI Policy After Hallucinated Citations:** # South Africa Pulls Ai Policy After Hallucinated Citations Expose Drafting Scandal ## Key Points - South Africa’s AI policy was pulled after AI hallucinations — https://www.cnbcafrica.com/2026/south-africa-pulls-ai-policy-after-hallucinated-citations-expose-drafting-scandal

<details><summary>Log</summary>

```
[2026-11-05T08:00:02.139Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-05T08:00:02.141Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-05T08:00:09.267Z] [africa] web search gathered 18 candidates (quality-filtered).
[2026-11-05T08:00:12.550Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-11-05T08:00:12.635Z] [history] 117 URLs posted in last 7d
[2026-11-05T08:00:12.637Z] [history] skip already-posted iafrica.com
[2026-11-05T08:00:12.638Z] [history] skip already-posted techinafrica.com
[2026-11-05T08:00:12.638Z] [history] skip already-posted daily.dev
[2026-11-05T08:00:12.638Z] [history] skip already-posted daily.dev
[2026-11-05T08:00:12.638Z] [history] skip already-posted daily.dev
[2026-11-05T08:00:12.638Z] [history] skip already-posted app.daily.dev
[2026-11-05T08:00:12.639Z] [history] skip already-posted reuters.com
[2026-11-05T08:00:12.639Z] [history] skip already-posted ainowinstitute.org
[2026-11-05T08:00:12.639Z] [history] skip already-posted facebook.com
[2026-11-05T08:00:12.640Z] [history] skip already-posted africaaisummit.org
[2026-11-05T08:00:12.651Z] [filter] deduped 26 → 16 (spam/history removed)
[2026-11-05T08:00:14.194Z] [enrich] arstechnica.com 84 → 985 chars
[2026-11-05T08:00:14.770Z] [enrich] techinafrica.com 116 → 1017 chars
[2026-11-05T08:00:14.930Z] [enrich] iafrica.com 117 → 1018 chars
[2026-11-05T08:00:14.947Z] [enrich] iafrica.com 118 → 1019 chars
[2026-11-05T08:00:15.091Z] [enrich] iafrica.com 104 → 1005 chars
[2026-11-05T08:00:15.943Z] [enrich] iafrica.com 92 → 993 chars
[2026-11-05T08:00:19.530Z] [quality] scored 12 candidates — top: #1:10 Strong South African focus, specific AI  | #2:10 Pan-African focus on AI health data, hig | #4:10 Southern African focus on AI skills gap,
[2026-11-05T08:00:19.530Z] Picked 12 candidates (top score 10) — drafting the BREAKING NEWS card.
[2026-11-05T08:00:21.673Z] [metrics] africa candidates=12 picked=https://www.cnbcafrica.com/2026/south-africa-pulls-ai-policy-after-hallucinated-citations-expose-drafting-scandal score=10 domains=iafrica.com,iafrica.com,iafrica.com,iafrica.com,cnbcafrica.com,facebook.com,techinafrica.com,arstechnica.com
[2026-11-05T08:00:22.834Z] Telegram post failed: telegram: Bad Request: chat not found
```
</details>
