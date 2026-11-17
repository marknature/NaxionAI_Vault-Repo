---
type: job
title: Weekend AI digest
slug: weekend-ai-digest-1beba57d
created: 2026-11-11T11:05:09.246Z
jobId: 1beba57d-6db7-41a2-aedb-2ec855d9ecab
status: succeeded
template: weekend-digest
persona: naxie
personaName: Naxie
startedAt: 2026-11-11T10:57:55.092Z
finishedAt: 2026-11-11T11:05:09.245Z
---

# Weekend AI digest

- **Status:** succeeded
- **Template:** weekend-digest
- **Started:** 2026-11-11T10:57:55.092Z
- **Finished:** 2026-11-11T11:05:09.245Z
- **Title:** Weekend AI digest

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Sweep all feeds — `pipeline` (77.8s)
2. ✓ Dedupe + rank — `pipeline` (212.3s)
3. ✓ Build weekend card — `pipeline` (432.9s)
4. ✓ Post to Telegram — `pipeline` (434.1s)

## Answer
🌴 WEEKEND AI DIGEST — 2026-11-11
2-sentence factual summary: Nvidia’s crisis has drawn attention from corporate governance experts who are considering the company's leadership and decision-making processes. This includes the recent controversy over Nvidia's acquisition of Arm.
Enjoy your weekend, here's to new opportunities and challenges in the tech world!

<details><summary>Log</summary>

```
[2026-11-11T10:57:55.105Z] Weekend sweep: Africa + World queries in one pass.
[2026-11-11T10:58:03.931Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-11T10:59:12.920Z] [weekend] web search gathered 18 candidates (quality-filtered).
[2026-11-11T10:59:14.284Z] [history] 130 URLs posted in last 7d
[2026-11-11T10:59:14.286Z] [history] skip already-posted whitehouse.gov
[2026-11-11T10:59:14.286Z] [history] skip already-posted nextgov.com
[2026-11-11T10:59:14.305Z] [history] skip already-posted wiley.law
[2026-11-11T10:59:14.305Z] [history] skip already-posted medium.com
[2026-11-11T10:59:14.305Z] [history] skip already-posted blog.intimetec.com
[2026-11-11T10:59:14.305Z] [history] skip already-posted reuters.com
[2026-11-11T10:59:14.305Z] [history] skip already-posted ainowinstitute.org
[2026-11-11T10:59:14.305Z] [history] skip already-posted cnbcafrica.com
[2026-11-11T10:59:14.305Z] [history] skip already-posted facebook.com
[2026-11-11T10:59:14.338Z] [filter] deduped 26 → 17 (spam/history removed)
[2026-11-11T11:00:00.198Z] [enrich] techcabal.com 94 → 995 chars
[2026-11-11T11:00:02.182Z] [enrich] blogs.nvidia.com 89 → 990 chars
[2026-11-11T11:01:27.381Z] [quality] scored 1 candidates — top: #1:8 one line | #2:7  | #3:7 
[2026-11-11T11:01:27.381Z] Picked 3 stories for the weekend card.
[2026-11-11T11:05:08.021Z] [metrics] weekend candidates=17 picked=https://techcrunch.com/2026/11/10/nvidias-crisis-has-corporate-governance-experts-reaching-for-the-popcorn/ score=8 domains=techcrunch.com,ventureburn.com,ventureburn.com,techcabal.com,techcabal.com,blogs.nvidia.com,blog.google,techcabal.com
[2026-11-11T11:05:09.245Z] Posted weekend digest to Telegram chat 8767926406.
```
</details>
