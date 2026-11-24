---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-9512e08c
created: 2026-11-24T15:38:41.482Z
jobId: 9512e08c-5f27-4100-b6de-113d8644fe12
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-24T15:35:28.842Z
finishedAt: 2026-11-24T15:38:41.482Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-24T15:35:28.842Z
- **Finished:** 2026-11-24T15:38:41.482Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (7.6s)
2. ✓ Dedupe + enrich — `pipeline` (7.8s)
3. ✓ Quality rank — `pipeline` (121.3s)
4. ✓ Build news card — `pipeline` (191.7s)
5. ✓ Post to Telegram — `pipeline` (192.6s)

## Answer
🧠 DAILY AI NEWS — Africa

South Africa to Draft National AI Action Plan in 90 Days, Ramaphosa Says

President Cyril Ramaphosa has directed that South Africa produce a National AI Action Plan within 90 days. The mandate signals a shift from policy discussion to time-bound execution at the highest level of government. Parliament and relevant departments are now expected to coordinate the drafting process. The plan will likely shape regulation, skills development, and public-sector adoption across the continent's most industrialised economy.

Why it matters for Africa
A presidential deadline turns AI governance into an urgent delivery target rather than an open-ended consultation. South Africa's approach often sets the template for regional peers, so the 90-day sprint could accelerate comparable frameworks across the SADC bloc.

📰 Read more: https://iafrica.com/south-africa-to-draft-national-ai-action-plan-in-90-days-ramaphosa-says/

#AI #Africa #AINews #SouthAfrica #AIPolicy #Ramaphosa

Source: web + innovation leads (RSS ≤48h + web + leads)
Story: **South Africa to Draft National AI Action Plan in 90 Days, Ramaphosa Says:** [iAfrica · 2026-11-24] South Africa to Draft National AI Action Plan in 90 Days, Ramaphosa Says — https://iafrica.com/south-africa-to-draft-national-ai-action-plan-in-90-days-ramaphosa-says/

<details><summary>Log</summary>

```
[2026-11-24T15:35:28.872Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-24T15:35:28.873Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-24T15:35:35.115Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-11-24T15:35:36.467Z] [africa] web search gathered 14 candidates (quality-filtered).
[2026-11-24T15:35:36.689Z] [history] 184 URLs posted in last 7d
[2026-11-24T15:35:36.692Z] [history] skip already-posted daily.dev
[2026-11-24T15:35:36.693Z] [history] skip already-posted daily.dev
[2026-11-24T15:35:36.693Z] [history] skip already-posted daily.dev
[2026-11-24T15:35:36.693Z] [history] skip already-posted app.daily.dev
[2026-11-24T15:35:36.693Z] [history] skip already-posted reuters.com
[2026-11-24T15:35:36.693Z] [history] skip already-posted cnbcafrica.com
[2026-11-24T15:35:36.709Z] [filter] deduped 22 → 16 (spam/history removed)
[2026-11-24T15:35:37.516Z] [enrich] iafrica.com 97 → 998 chars
[2026-11-24T15:35:37.521Z] [enrich] iafrica.com 113 → 1014 chars
[2026-11-24T15:35:48.085Z] [enrich] arstechnica.com 108 → 1009 chars
[2026-11-24T15:35:50.277Z] [enrich] africaainews.com 105 → 1006 chars
[2026-11-24T15:35:50.915Z] [enrich] techinafrica.com 139 → 1040 chars
[2026-11-24T15:35:54.628Z] [enrich] iafrica.com 95 → 231 chars
[2026-11-24T15:37:30.164Z] [quality] scored 1 candidates — top: #1:10 Zimbabwe-specific AI initiative with rec | #2:9  | #3:9 
[2026-11-24T15:37:30.165Z] Picked 12 fresh candidates (top score 10) — drafting the daily card.
[2026-11-24T15:38:40.622Z] [metrics] africa candidates=12 picked=https://iafrica.com/south-africa-to-draft-national-ai-action-plan-in-90-days-ramaphosa-says/ score=9 domains=techinafrica.com,iafrica.com,arstechnica.com,africaainews.com,iafrica.com,iafrica.com,iafrica.com,theverge.com
[2026-11-24T15:38:41.481Z] Posted Africa BREAKING NEWS to Telegram chat -1004307136262.
```
</details>
