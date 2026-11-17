---
type: job
title: Africa AI news — BREAKING
slug: africa-ai-news-breaking-71079df5
created: 2026-11-13T10:54:37.129Z
jobId: 71079df5-993a-4220-8573-99b5b85ac823
status: succeeded
template: africa-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-13T10:34:11.170Z
finishedAt: 2026-11-13T10:54:37.129Z
---

# Africa AI news — BREAKING

- **Status:** succeeded
- **Template:** africa-ai-news
- **Started:** 2026-11-13T10:34:11.170Z
- **Finished:** 2026-11-13T10:54:37.129Z
- **Title:** Africa AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web + leads — `pipeline` (33.8s)
2. ✓ Dedupe + enrich — `pipeline` (33.8s)
3. ✓ Quality rank — `pipeline` (400.8s)
4. ✓ Build news card — `pipeline` (1215.8s)
5. ✓ Post to Telegram — `pipeline` (1226.0s)

## Answer
🧠 DAILY AI NEWS — Africa

Vodacom Seeks Partners to Build AI Data Centres in South Africa and Kenya

Vodacom, a major South African telecommunications company, is seeking partners to build AI data centres in both South Africa and Kenya. This initiative aims to leverage AI technology to enhance services and support economic growth in the region.

Why it matters for Africa
By partnering with Vodacom, potential AI data centre operators can tap into the growing market in Africa, where AI applications are expected to significantly impact various sectors including healthcare, finance, and education.

📰 Read more: https://iafrica.com/vodacom-seeks-partners-to-build-ai-data-centres-in-south-africa-and-kenya/

#AI #Africa #AINews #Vodacom #DataCentres

Source: web + innovation leads (RSS ≤48h + web + leads)
Story: **Vodacom Seeks Partners to Build AI Data Centres in South Africa and Kenya:** [iAfrica · 2026-11-12] Vodacom Seeks Partners to Build AI Data Centres in South Africa and Kenya Vodacom Seeks Partners to Build AI Data Centres in South Africa — https://iafrica.com/vodacom-seeks-partners-to-build-ai-data-centres-in-south-africa-and-kenya/

<details><summary>Log</summary>

```
[2026-11-13T10:34:11.180Z] Sweeping for today's Africa/AI news (web + innovation leads).
[2026-11-13T10:34:11.180Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-11-13T10:34:19.034Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-11-13T10:34:44.983Z] [africa] web search gathered 15 candidates (quality-filtered).
[2026-11-13T10:34:45.009Z] [history] 140 URLs posted in last 7d
[2026-11-13T10:34:45.010Z] [history] skip already-posted iafrica.com
[2026-11-13T10:34:45.014Z] [filter] deduped 23 → 22 (spam/history removed)
[2026-11-13T10:35:00.140Z] [enrich] techcabal.com 100 → 843 chars
[2026-11-13T10:35:00.141Z] [enrich] iafrica.com 96 → 285 chars
[2026-11-13T10:35:01.225Z] [enrich] techcabal.com 77 → 820 chars
[2026-11-13T10:35:02.245Z] [enrich] iafrica.com 79 → 234 chars
[2026-11-13T10:35:02.246Z] [enrich] techcabal.com 94 → 837 chars
[2026-11-13T10:35:03.526Z] [enrich] techcabal.com 85 → 828 chars
[2026-11-13T10:40:52.002Z] [quality] scored 1 candidates — top: #1:10 African angle FIRST, AI/Tech core, recen | #2:9  | #3:9 
[2026-11-13T10:40:52.003Z] Picked 12 fresh candidates (top score 10) — drafting the daily card.
[2026-11-13T10:54:27.028Z] [metrics] africa candidates=12 picked=https://iafrica.com/vodacom-seeks-partners-to-build-ai-data-centres-in-south-africa-and-kenya/ score=9 domains=techcabal.com,iafrica.com,techcabal.com,techcabal.com,iafrica.com,techcabal.com,techcabal.com,worldatlas.com
[2026-11-13T10:54:37.129Z] Telegram post failed: telegram send failed: fetch failed
```
</details>
