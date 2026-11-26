---
personaId: "social-media-manager"
taskId: "sasha-comments"
completedAt: "2026-11-26T10:03:51.425Z"
runId: "b8eee770-730a-4c7d-8a47-f7b3f65720c1"
---

# Comment monitoring

Completed by social-media-manager.

Naxie · Sasha

**Answer: Cannot execute — no live account access or mention data provided**

The vault notes show this is a recurring research task title, but they contain **no actual mention/comment data, account handles, or platform credentials** to analyze. The web sources describe *tools and methodologies* for social monitoring, not your specific accounts.

**What would be needed to fulfill this request:**
1. **Account access** — API tokens or authenticated connections to X, LinkedIn, Instagram, etc. (governed by *Information Security Handling Policy*: credentials live in Integrations store, never in prompts)
2. **Mention/comment export** — Raw data (CSV/JSON) from each platform covering the desired window
3. **Reply criteria** — Your rules for "needs a reply" (e.g., questions, complaints, high-engagement negative sentiment, untagged brand mentions)

**Available approaches (from sources):**
- **Free snapshot tools** (Sift AI [1]) — one-time scan of public posts by keyword/brand across X, TikTok, YouTube, Instagram, news; returns volume, themes, sentiment, top posts, CSV export
- **Enterprise platforms** (Sift, Hootsuite/Talkwalker [2], Sprout Social [3]) — continuous monitoring, AI triage ("what needs a reply"), crisis alerts, sentiment trends, share-of-voice
- **DIY pipeline** — Pull via platform APIs → normalize → sentiment model (VADER, transformer) → rule-based flagging → daily digest

**Governance guardrails:**
- *AI & Automation Acceptable-Use Policy*: No external posts/replies without recorded approval in Approvals queue
- *Social Media Publications Accuracy Policy*: Any public response must cite real, retrievable sources
- *Information Security Handling Policy*: Personal data in mentions must be redacted unless explicit consent recorded

**Next step:** Provide a data export (or grant read-only API access via Integrations) and your reply-flagging rules. I can then synthesize a sentiment summary and flag list — **but I will not post or reply without a separate approval record.**
