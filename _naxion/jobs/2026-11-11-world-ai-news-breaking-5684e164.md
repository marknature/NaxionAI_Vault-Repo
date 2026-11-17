---
type: job
title: World AI news — BREAKING
slug: world-ai-news-breaking-5684e164
created: 2026-11-11T08:32:50.148Z
jobId: 5684e164-1a31-42a7-8168-e3e81b62dcf2
status: succeeded
template: world-ai-news
persona: naxie
personaName: Naxie
startedAt: 2026-11-11T08:26:54.963Z
finishedAt: 2026-11-11T08:32:50.148Z
---

# World AI news — BREAKING

- **Status:** succeeded
- **Template:** world-ai-news
- **Started:** 2026-11-11T08:26:54.963Z
- **Finished:** 2026-11-11T08:32:50.148Z
- **Title:** World AI news — BREAKING

## Inputs
```json
{
  "dailyDigest": true,
  "chatId": "-1004307136262"
}
```

### Steps
1. ✓ Sweep RSS + web — `pipeline` (6.2s)
2. ✓ Dedupe + enrich — `pipeline` (6.2s)
3. ✓ Quality rank — `pipeline` (168.0s)
4. ✓ Build news card — `pipeline` (354.1s)
5. ✓ Post to Telegram — `pipeline` (355.2s)

## Answer
🧠 DAILY SUPER INTELLIGENCE / AI NEWS — World

LongCat-2.0: Trillion-Parameter AI Model Trained Without Nvidia Chips

LongCat-2.0, a 1.6-trillion-parameter Mixture-of-Experts model, was released by Meituan, a Beijing-based food-delivery giant, on June 30, 2026. The model completed both pretraining and inference entirely on a 50,000-chip cluster of domestic Chinese accelerators, believed to be Huawei’s Ascend line. This breakthrough demonstrates the potential for AI development without relying on Nvidia chips, which could significantly impact the global AI landscape.

Why it matters
LongCat-2.0 represents a significant leap in AI model training efficiency and scalability. It showcases the possibility of developing large-scale AI models using local resources, potentially reducing dependency on foreign technology and lowering costs. This could accelerate AI adoption in regions where access to advanced hardware is limited.

📰 Read more: https://medium.com/write-a-catalyst/12-real-ai-breakthroughs-from-mid-2026-fully-verified-2110a341ac28

#AI #SuperIntelligence #ChinaTech #Nvidia #Huawei

Source: RSS ≤48h + web search
Story: **LongCat-2.0: Trillion-Parameter AI Model Trained Without Nvidia Chips:** # 12 Real AI Breakthroughs From Mid-2026, Fully Verified ## 1. LongCat-2.0 — the first trillion-parameter model trained entirely without Nvidia chips Released J — https://medium.com/write-a-catalyst/12-real-ai-breakthroughs-from-mid-2026-fully-verified-2110a341ac28

<details><summary>Log</summary>

```
[2026-11-11T08:26:54.980Z] Sweeping for today's World AI news (RSS + web search).
[2026-11-11T08:26:54.980Z] [world] quality pipeline: RSS (≤48h) + web search → dedupe → enrich → quality rank
[2026-11-11T08:26:59.179Z] [world] web search gathered 14 candidates (quality-filtered).
[2026-11-11T08:27:01.174Z] [rss/world] curated feeds: 8 fresh items (≤48h).
[2026-11-11T08:27:01.198Z] [history] 127 URLs posted in last 7d
[2026-11-11T08:27:01.198Z] [history] skip already-posted whitehouse.gov
[2026-11-11T08:27:01.198Z] [history] skip already-posted nextgov.com
[2026-11-11T08:27:01.198Z] [history] skip already-posted wiley.law
[2026-11-11T08:27:01.198Z] [history] skip already-posted blog.intimetec.com
[2026-11-11T08:27:01.204Z] [filter] deduped 22 → 18 (spam/history removed)
[2026-11-11T08:27:03.402Z] [enrich] techcrunch.com 102 → 1003 chars
[2026-11-11T08:27:03.441Z] [enrich] ventureburn.com 97 → 631 chars
[2026-11-11T08:27:12.348Z] [enrich] techcabal.com 90 → 991 chars
[2026-11-11T08:27:12.523Z] [enrich] blogs.nvidia.com 89 → 990 chars
[2026-11-11T08:27:14.151Z] [enrich] huggingface.co 121 → 1022 chars
[2026-11-11T08:27:15.200Z] [enrich] openai.com 79 → 980 chars
[2026-11-11T08:29:43.016Z] [quality] scored 12 candidates — top: #9:9 7 days old, high novelty, tier1 press, h | #1:8 one line | #6:6 7 days old, niche focus, no source credi
[2026-11-11T08:29:43.016Z] Picked 12 fresh candidates (top score 9) — drafting the daily card.
[2026-11-11T08:32:49.113Z] [metrics] world candidates=12 picked=https://medium.com/write-a-catalyst/12-real-ai-breakthroughs-from-mid-2026-fully-verified-2110a341ac28 score=9 domains=medium.com,huggingface.co,openai.com,blogs.nvidia.com,facebook.com,youtube.com,facebook.com,aifundingtracker.com
[2026-11-11T08:32:50.148Z] Posted World BREAKING NEWS to Telegram chat -1004307136262.
```
</details>
