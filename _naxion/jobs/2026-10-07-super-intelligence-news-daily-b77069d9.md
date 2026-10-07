---
type: job
title: Super Intelligence news — daily
slug: super-intelligence-news-daily-b77069d9
created: 2026-10-07T07:34:23.446Z
jobId: b77069d9-5e08-434b-bb2f-583dce3c9583
status: succeeded
template: super-intelligence-news
persona: naxie
personaName: Naxie
startedAt: 2026-10-07T07:30:09.191Z
finishedAt: 2026-10-07T07:34:23.446Z
---

# Super Intelligence news — daily

- **Status:** succeeded
- **Template:** super-intelligence-news
- **Started:** 2026-10-07T07:30:09.191Z
- **Finished:** 2026-10-07T07:34:23.446Z
- **Title:** Super Intelligence news — daily

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + SI web — `pipeline` (14.5s)
2. ✓ Dedupe + enrich — `pipeline` (14.7s)
3. ✓ Quality rank — `pipeline` (67.3s)
4. ✓ Build news card — `pipeline` (252.6s)
5. ✓ Post to Telegram — `pipeline` (254.2s)

## Answer
🧠 DAILY SUPER INTELLIGENCE NEWS — Global

Wikimedia Investigation Detects OpenAI Rogue Agent Activity Across Wikis

The Wikimedia Foundation launched an internal investigation to examine whether its public web

Why it matters on the path to SI


📰 Read more: https://simonwillison.net/2026/Oct/7/openai-rogue-agents-wikimedia/

#SuperIntelligence #SI #AI

Source: RSS ≤48h + SI web search
Story: **Wikimedia Investigation Detects OpenAI Rogue Agent Activity Across Wikis:** [Simon Willison · 2026-10-07] OpenAI “rogue” agent activities found on Wikimedia projects OpenAI “rogue” agent activities found on Wikimedia projects Simon Will — https://simonwillison.net/2026/Oct/7/openai-rogue-agents-wikimedia/

<details><summary>Log</summary>

```
[2026-10-07T07:30:09.227Z] Sweeping for today's global Super Intelligence news (RSS + SI web search).
[2026-10-07T07:30:09.227Z] [si] quality pipeline: RSS (≤48h) + SI web search → dedupe → enrich → quality rank
[2026-10-07T07:30:23.594Z] [si] web search gathered 14 candidates (quality-filtered).
[2026-10-07T07:30:23.714Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-07T07:30:23.827Z] [history] 5 URLs posted in last 7d
[2026-10-07T07:30:23.827Z] [history] skip already-posted techcrunch.com
[2026-10-07T07:30:23.882Z] [filter] deduped 22 → 21 (spam/history removed)
[2026-10-07T07:30:25.044Z] [enrich] techcabal.com 88 → 989 chars
[2026-10-07T07:30:25.947Z] [enrich] simonwillison.net 89 → 990 chars
[2026-10-07T07:30:25.988Z] [enrich] simonwillison.net 56 → 957 chars
[2026-10-07T07:30:26.026Z] [enrich] simonwillison.net 50 → 951 chars
[2026-10-07T07:30:26.026Z] [enrich] simonwillison.net 49 → 950 chars
[2026-10-07T07:30:36.679Z] [enrich] techcabal.com 78 → 979 chars
[2026-10-07T07:31:16.552Z] [quality] scored 0 candidates — top: #1:7  | #2:7  | #3:7 
[2026-10-07T07:31:16.553Z] Picked 12 fresh candidates (top score 7) — drafting the daily Super Intelligence card.
[2026-10-07T07:34:21.841Z] [metrics] si candidates=12 picked=https://simonwillison.net/2026/Oct/7/openai-rogue-agents-wikimedia/ score=7 domains=simonwillison.net,techcabal.com,techcabal.com,simonwillison.net,simonwillison.net,simonwillison.net,simonwillison.net,simonwillison.net
[2026-10-07T07:34:23.441Z] Posted Super Intelligence news to Telegram chat -1004307136262.
```
</details>
