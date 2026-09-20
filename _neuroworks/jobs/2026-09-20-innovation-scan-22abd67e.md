---
type: job
title: Innovation scan
slug: innovation-scan-22abd67e
created: 2026-09-20T04:07:10.957Z
jobId: 22abd67e-d57a-413d-a544-b85ccc63a218
status: succeeded
template: innovation-scan
persona: clawbot
personaName: Neuro
startedAt: 2026-09-20T04:00:21.388Z
finishedAt: 2026-09-20T04:07:10.957Z
---

# Innovation scan

- **Status:** succeeded
- **Template:** innovation-scan
- **Started:** 2026-09-20T04:00:21.388Z
- **Finished:** 2026-09-20T04:07:10.957Z
- **Title:** Innovation scan

## Plan
Find "REPORT RAG" in documents

### Steps
1. ✓ Looking in your documents for "REPORT RAG" — `fs.find_in` (0.0s)
    > default fallback: task mentions document — search the user's PC instead of the web
2. ✓ Quality-checking the draft — `quality.check` (18.1s)
    > auto-injected: score factuality, citation coverage, persona fit (evidence-aware)
3. ✓ Security-scanning the note — `security.scan` (0.0s)
    > auto-injected: scan answer for secrets, dodgy URLs

## Answer
## Summary
The primary opportunity for the platform is the transition from passive RAG to **Agentic Reflection**, specifically to address the current system health plateau and vault stagnation [Note 1]. The overall theme of this scan is "System Autonomy"—moving beyond simple task execution to self-healing pipelines that manage their own data hygiene and model routing. Immediate action should be taken to integrate Gemini as a secondary cloud router and implement an automated cleanup agent to process the 99 dormant files currently dragging down system health [Note 1, Note 5].

## Top 3 opportunities

1.  **Automated Vault Janitor (Self-Correction Agent)**
    *   **What it is:** A dedicated agentic loop that scans the knowledge vault for "dormant" files, summarizes them for archival, or deletes redundant stubs to improve RAG retrieval quality.
    *   **Why it helps:** Directly addresses the 61/100 health plateau and the 99 dormant files identified in recent audits [Note 1].
    *   **Effort:** M (Requires a deterministic plan builder to avoid accidental data loss).

2.  **Multi-Provider Cloud Routing (Gemini Integration)**
    *   **What it is:** Expanding the cloud-routing layer to include Google Gemini models alongside existing providers.
    *   **Why it helps:** Fulfills specific operator requests for Gemini usage and provides a fallback when other cloud synthesisers exceed time limits [Note 5, Note 3].
    *   **Effort:** S (Standard API integration within the existing routed LLM layer).

3.  **WhatsApp-Based Human-in-the-Loop (HITL)**
    *   **What it is:** Integrating a WhatsApp API gateway (e.g., Twilio or Paynow) to allow the operator to approve agent plans or answer queries via mobile.
    *   **Why it helps:** Critical for Zimbabwean SMEs where mobile data is more persistent than desktop uptime; it ensures the "human-in-the-loop" layer is always accessible.
    *   **Effort:** M (Requires webhook handling and state management for asynchronous approvals).

## Agent & AI techniques
*   **Agentic RAG:** Moving from simple vector search to a multi-step process where the agent evaluates the relevance of retrieved context before answering. This prevents the "research synth exceeded 120s" failures seen in recent sessions by allowing the agent to refine its search query mid-stream [Note 3].
*   **Reflection & Self-Critique:** Implementing a "critic" agent that reviews the output of the "planner" agent. This is essential for maintaining the "strict" validator standards seen in the vault notes [Note 1].
*   **Local-First Small Language Models (SLMs):** Utilizing Llama 3.2 or Mistral (via Ollama) for the "Janitor" tasks. These models are now efficient enough to handle data classification locally, saving cloud costs for high-reasoning tasks.

## APIs
*   **Paynow (Zimbabwe):** Essential for local SMEs to handle automated invoicing or payment triggers directly from agentic workflows.
*   **OpenRouter:** To provide a unified interface for the requested Gemini models and other emerging LLMs without individual API management.
*   **Twilio/MessageBird:** For the WhatsApp HITL layer, providing robust delivery in the local region.

## GitHub repos
*   **LangGraph (by LangChain):** A library for building stateful, multi-agent applications with cyclic graphs. *License: MIT. Activity: High (Daily commits).*
*   **RAGFlow:** An open-source deep RAG engine based on deep document understanding. *License: Apache-2.0. Activity: Very Active.*
*   **Crawl4AI:** A fast, agent-friendly web crawler that outputs clean Markdown, ideal for the "shallow web pass" requirements. *License: Apache-2.0. Activity: Trending.*

## Signals from our own usage
*   **System Health Decline:** The MD System Audit has plateaued at 61/100, indicating that current deterministic builders are not keeping up with vault growth [Note 1].
*   **Data Stagnation:** There are 99 dormant files in the system, suggesting the "Knowledge Vault" is accumulating noise that needs an automated cleanup strategy [Note 1].
*   **Pipeline Stalls:** The "Todo Brief" has reported 0 open tasks for five consecutive days, which may indicate a failure in the task ingestion or scheduling layer rather than a lack of work [Note 1].
*   **Model Preference:** There is an explicit operator request to "use Gemini this time" for research tasks, suggesting the current cloud routing may be underperforming or hitting limits [Note 5].

## Watchlist
*   **Durable Agent Memory (MAG):** While "MAG" is mentioned in several notes, the current implementation seems to struggle with synthesis timeouts [Note 3, Note 5]. This requires monitoring but not a full rebuild yet.
*   **Local Vision Models:** Using Ollama-based vision models to "read" screenshots of system errors, which could eventually automate the "System Health" audit process further.

_Assumed: The "Zimbabwean SME" context was prioritized for API selection based on the platform's stated workforce goals._

<details><summary>Log</summary>

```
[2026-09-20T04:00:21.396Z] Read 8 recent inbox notes from the vault as local signal.
[2026-09-20T04:00:21.397Z] Working as Neuro — AI agent operator.
[2026-09-20T04:00:21.409Z] Reading your Gmail inbox (recent) — up to 9 messages.
[2026-09-20T04:00:21.410Z] Recognised the shape — Direct tool use, 1 step.
[2026-09-20T04:00:21.412Z] Plan repair: rerouting from web/vault search to local-PC search — task mentions document.
[2026-09-20T04:00:21.413Z] Plan ready: 1 step — Find "REPORT RAG" in documents.
[2026-09-20T04:00:21.430Z] Running with help from 2 peer workers (capacity 7 thinking + 8 I/O sub-agents).
[2026-09-20T04:00:21.431Z] Step 1 of 1: Looking in your documents for "REPORT RAG"
[2026-09-20T04:00:21.445Z] All sub-agents finished in 0.0s.
[2026-09-20T04:00:21.601Z] Thinking with gemini-3-flash-preview (~9,605 tokens of context). Reason: profile "synthesis" + complex task — handoff to large model gemini-3-flash-preview.
[2026-09-20T04:00:37.528Z] Reviewing the draft — running quality and security checks in parallel.
[2026-09-20T04:00:37.535Z] Running with help from 2 peer workers (capacity 7 thinking + 8 I/O sub-agents).
[2026-09-20T04:00:37.535Z] Running 2 sub-agents in parallel (1 I/O + 1 thinking).
[2026-09-20T04:00:37.535Z] Step 3 of 3: Security-scanning the note
[2026-09-20T04:00:37.536Z] Step 2 of 3: Quality-checking the draft
[2026-09-20T04:00:55.701Z] Wave 1 finished in 18.2s.
[2026-09-20T04:00:55.701Z] All sub-agents finished in 18.2s.
[2026-09-20T04:00:55.701Z] Quality check passed (87%) and security is clean — peer review skipped (saves 30-90s).
[2026-09-20T04:00:55.702Z] [africa] quality pipeline: RSS (≤48h) + web search + innovation leads → dedupe → enrich → quality rank
[2026-09-20T04:00:59.867Z] [rss/africa] curated feeds: 8 fresh items (≤48h).
[2026-09-20T04:01:02.143Z] [africa] web search gathered 14 candidates (quality-filtered).
[2026-09-20T04:01:02.144Z] [africa] +1 innovation-scan leads
[2026-09-20T04:01:02.147Z] [history] 8 URLs posted in last 7d
[2026-09-20T04:01:02.531Z] [enrich] ventureburn.com 101 → 738 chars
[2026-09-20T04:01:02.652Z] [enrich] techinafrica.com 97 → 566 chars
[2026-09-20T04:01:07.777Z] [enrich] techinafrica.com 144 → 1045 chars
[2026-09-20T04:01:09.383Z] [enrich] techcabal.com 103 → 1004 chars
[2026-09-20T04:01:09.480Z] [enrich] techcabal.com 94 → 995 chars
[2026-09-20T04:01:09.498Z] [enrich] techcabal.com 104 → 1005 chars
[2026-09-20T04:04:26.887Z] [quality] scored 12 candidates — top: #6:9 Africa angle is high, source credibility | #2:8 Africa angle is high, source credibility | #3:8 Africa angle is high, source credibility
[2026-09-20T04:07:10.956Z] Saved 6 story leads for the daily social posts (_neuroworks/social/story-leads.md).
```
</details>
