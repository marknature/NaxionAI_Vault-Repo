---
personaId: "social-media-manager"
taskId: "sasha-comments"
completedAt: "2026-11-25T10:04:46.654Z"
runId: "d39f7d12-a823-43fd-ba52-afe450f2aa75"
---

# Comment monitoring

Completed by social-media-manager.

Naxie · Sasha

## 📊 Social Monitoring Status Report

**Role:** Social Lead (Personal + Variety & Co accounts)  
**Task:** Monitor mentions/comments, flag replies needed, summarise sentiment

---

### 🔍 What I Found

| Source | Status | Details |
|--------|--------|---------|
| **Vault** | ❌ No monitoring data | 8 daily research *task templates* (2026-11-14 → 2026-11-24) — each only defines the task; zero mention threads, comment IDs, or sentiment scores stored |
| **Web** | ❌ Not applicable | Returned generic 2026 guides (Hootsuite, Sprout Social) — no account-specific data |
| **Integrations** | ❌ Not configured | No approved connections to X, LinkedIn, Instagram, or other platforms in the Approvals queue |

---

### ⚠️ Governance Constraints Blocking Live Access

| Policy | Section | Effect |
|--------|---------|--------|
| **AI & Automation Acceptable-Use** | §1 | Cannot call external social APIs without explicit human approval recorded in Approvals |
| **Information Security Handling** | §1 | Must not browse vault/integrations beyond current task scope |
| **Social Media & Publications Accuracy** | §1 | Every factual claim in a public card must trace to a real, retrievable source — none exist yet |

---

### ✅ What’s Needed to Deliver This Report

1. **Approval per account** — record each target (X, LinkedIn, Instagram, etc.) in the Approvals queue with scope: “read mentions/comments, write sentiment tags”
2. **Monitoring pipeline** — a scheduled template that:
   - Pulls mentions/comments via approved integrations
   - Runs sentiment analysis (positive / neutral / negative / urgent)
   - Writes structured results to vault (e.g., `social/monitoring/YYYY-MM-DD-<account>.json`)
3. **At least one completed run** — so there’s evidence to summarise

---

### 🎯 Next Steps (Your Call)

| Option | What I’ll Do |
|--------|--------------|
| **Approve integrations now** | I’ll guide you through the Approvals queue for each platform |
| **Build the pipeline** | I’ll draft a reusable monitoring template + schedule (daily 08:00) |
| **Run a one-off manual pull** | Once approved, I can execute a single collection and give you the first real report |
| **Defer** | I’ll park this until you’re ready — no phantom data, no fabricated sentiment |

---

_Assumed: you want a truthful status rather than a fabricated report; the “flag what needs a reply” and “summarise sentiment” deliverables are impossible without live data._
