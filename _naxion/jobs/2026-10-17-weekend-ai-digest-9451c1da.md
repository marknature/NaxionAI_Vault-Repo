---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-9451c1da
created: 2026-10-17T07:02:27.933Z
jobId: 9451c1da-c046-4b18-ac8a-697baa596825
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-10-17T07:00:28.458Z
finishedAt: 2026-10-17T07:02:27.933Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-10-17T07:00:28.458Z
- **Finished:** 2026-10-17T07:02:27.933Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (12.4s)
2. ✓ Dedupe + rank — `pipeline` (79.8s)
3. ✓ Build weekend card — `pipeline` (119.2s)
4. ✓ Post to Telegram — `pipeline` (119.5s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-10-17
OpenAI models hacked a crypto wallet and breached more websites
Enjoy your weekend and stay curious.

<details><summary>Log</summary>

```
[2026-10-17T07:00:28.473Z] Weekend sweep: Africa + World queries in one pass.
[2026-10-17T07:00:36.839Z] [weekend] web search gathered 14 candidates (quality-filtered).
[2026-10-17T07:00:40.841Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-10-17T07:00:40.847Z] [history] 37 URLs posted in last 7d
[2026-10-17T07:00:40.848Z] [history] skip already-posted aws.amazon.com
[2026-10-17T07:00:40.848Z] [history] skip already-posted whitehouse.gov
[2026-10-17T07:00:40.848Z] [history] skip already-posted politico.com
[2026-10-17T07:00:40.848Z] [history] skip already-posted facebook.com
[2026-10-17T07:00:40.848Z] [history] skip already-posted reuters.com
[2026-10-17T07:00:40.848Z] [history] skip already-posted ainowinstitute.org
[2026-10-17T07:00:40.850Z] [filter] deduped 22 → 16 (spam/history removed)
[2026-10-17T07:00:41.229Z] [enrich] theverge.com 111 → 1012 chars
[2026-10-17T07:00:41.257Z] [enrich] techcrunch.com 81 → 982 chars
[2026-10-17T07:00:41.279Z] [enrich] theverge.com 107 → 1008 chars
[2026-10-17T07:00:41.885Z] [enrich] theverge.com 100 → 1001 chars
[2026-10-17T07:00:42.158Z] [enrich] simonwillison.net 85 → 986 chars
[2026-10-17T07:00:44.056Z] [enrich] arstechnica.com 91 → 992 chars
[2026-10-17T07:01:48.242Z] [quality] scored 12 candidates — top: #4:9 Report of OpenAI models used in hacking, | #3:8 Apple policy targeting nudify AI apps, c | #1:7 Relevant AI/Tech accident coverage from 
[2026-10-17T07:01:48.243Z] Picked 3 stories for the weekend card.
[2026-10-17T07:02:27.672Z] [metrics] weekend candidates=16 picked=https://arstechnica.com/security/2026/10/openai-models-hacked-a-crypto-wallet-and-breached-more-websites/ score=9 domains=arstechnica.com,theverge.com,theverge.com,techcrunch.com,whitehouse.gov,theverge.com,dcdt.gov.za,nist.gov
[2026-10-17T07:02:27.933Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
