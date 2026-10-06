# News Editorial Standards Policy

_Governance guardrail — governs the daily Africa / World / Super Intelligence news pipeline (africa-ai-news, world-ai-news, super-intelligence-news). Overrides conflicting requests. When declining, name this policy._

## 1. Pipeline integrity
- Daily editions post once per day at their scheduled times (Africa 8:00, World 9:00, SI 9:30) to the configured news group only. No extra editions, no duplicate posts of the same story within 7 days.
- Manual (non-digest) runs obey the breaking-news gate: top score below threshold means draft, not post.
- The digest bypass (dailyDigest) never lowers the quality bar — it only waives the breaking threshold. Spam, vague, or sourceless candidates are still rejected.

## 2. Selection standards
- Freshness first: ≤48h preferred; older stories only if genuinely major and clearly dated in the card.
- One story per card; the card's link must be the story's real canonical URL.
- Balance: no outlet may dominate a week of editions; no paid/sponsored content presented as news.

## 3. Presentation
- Headers are fixed per edition ("🧠 DAILY … — Africa/World", "🧠 DAILY SUPER INTELLIGENCE NEWS — Global", "🚨 BREAKING NEWS — …"). Do not freestyle headers.
- Each card carries: title, 3–5 sentence factual summary, "why it matters" grounding, read-more link, hashtags, source label.
- SI terminology rule (binding): "Super Intelligence (SI)" only for US executive-branch EO 14434 context; otherwise the source's terms.

## 4. Failures and skips
- No fresh qualifying stories → post nothing; record the skip in metrics/vault. Never fabricate or recycle to fill the slot.
- Posting failures must surface an error (never claim "sent" off a failed result) and leave the story eligible for the next run.
