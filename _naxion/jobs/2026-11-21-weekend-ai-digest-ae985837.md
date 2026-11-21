---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-ae985837
created: 2026-11-21T07:07:36.990Z
jobId: ae985837-0a00-4294-9bba-4ca1f573925f
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-11-21T07:00:16.821Z
finishedAt: 2026-11-21T07:07:36.990Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-11-21T07:00:16.821Z
- **Finished:** 2026-11-21T07:07:36.990Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (84.6s)
2. ✓ Dedupe + rank — `pipeline` (309.6s)
3. ✓ Build weekend card — `pipeline` (438.9s)
4. ✓ Post to Telegram — `pipeline` (440.1s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-11-21
One endpoint across Regions and clusters for Amazon SageMaker's Global Inference Gateway
Enjoy your weekend, here’s to relaxing and exploring the latest in AI and beyond!

<details><summary>Log</summary>

```
[2026-11-21T07:00:16.858Z] Weekend sweep: Africa + World queries in one pass.
[2026-11-21T07:00:26.912Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-21T07:01:41.448Z] [weekend] web search gathered 12 candidates (quality-filtered).
[2026-11-21T07:01:41.488Z] [history] 174 URLs posted in last 7d
[2026-11-21T07:01:41.488Z] [history] skip already-posted aws.amazon.com
[2026-11-21T07:01:41.489Z] [history] skip already-posted openai.com
[2026-11-21T07:01:41.497Z] [filter] deduped 20 → 18 (spam/history removed)
[2026-11-21T07:01:41.520Z] [enrich] aws.amazon.com 135 → 1036 chars
[2026-11-21T07:01:41.520Z] [enrich] aws.amazon.com 145 → 1046 chars
[2026-11-21T07:01:41.520Z] [enrich] aws.amazon.com 121 → 1022 chars
[2026-11-21T07:01:41.565Z] [enrich] arstechnica.com 112 → 1013 chars
[2026-11-21T07:01:51.777Z] [enrich] arstechnica.com 102 → 1003 chars
[2026-11-21T07:01:52.842Z] [enrich] arstechnica.com 106 → 1007 chars
[2026-11-21T07:05:26.411Z] [quality] scored 1 candidates — top: #1:8 Relevant to global AI/Tech, recent, from | #2:7  | #3:7 
[2026-11-21T07:05:26.412Z] Picked 3 stories for the weekend card.
[2026-11-21T07:07:35.751Z] [metrics] weekend candidates=18 picked=https://aws.amazon.com/blogs/machine-learning/introducing-amazon-sagemaker-hyperpod-global-inference-gateway-one-endpoint-across-regions-and-clusters/ score=8 domains=aws.amazon.com,aws.amazon.com,aws.amazon.com,arstechnica.com,arstechnica.com,arstechnica.com,wired.com,britannica.com
[2026-11-21T07:07:36.989Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
