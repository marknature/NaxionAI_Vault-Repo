---
title: "Research: You are a Product Manager working on a sub-task of a larger orchestration.

YOUR SUB-TASK: Create a high‑level roadmap t"
created: 2026-10-04
source: naxie-research
validator: strict
sources_kept: 2
sources_dropped: 1
---

# Research: You are a Product Manager working on a sub-task of a larger orchestration.

YOUR SUB-TASK: Create a high‑level roadmap that outlines the sequence of improvement initiatives for Naxie over the next 12‑18 months. Include major milestones, estimated timeframes (quarters), and which type of improvement each milestone addresses (technical, UX, market, business). Output format: a simple Gantt‑style tabl

**Naxie 12‑18‑Month High‑Level Roadmap**

| Milestone (Goal) | Target Quarter* | Improvement Type |
|------------------|------------------|------------------|
| **Q4 2026 – Enable employee‑clock logging** – instrument the task runner so every sub‑agent run is attributed to a logged‑in employee. | Q4 2026 | Business / Technical |
| **Q4 2026 – Audit & fix zero‑duration templates** – verify that `todo‑brief`, `weekly‑rollup`, and other “0 s” tasks actually execute logic and record duration. | Q4 2026 | Technical / UX |
| **Q1 2027 – Split `innovation‑scan` into parallel sub‑agents** – break the 10‑min bottleneck into concurrent steps or trim heavy stages. | Q1 2027 | Technical |
| **Q1 2027 – Enrich skill metadata for `send‑attachment` & `brief‑writing`** – add richer intent phrases to raise picker confidence (currently weak scores). | Q1 2027 | UX / Technical |
| **Q2 2027 – Introduce low‑frequency, high‑complexity “Quarterly Strategy Scan”** – a deeper market‑analysis task that runs once per quarter to diversify workload. | Q2 2027 | Business / Market |
| **Q2 2027 – Deploy peer‑delegated task framework** – allow tasks to be handed off to other agents, testing load‑balancing across the fleet. | Q2 2027 | Business / Technical |
| **Q3 2027 – Integrate `web.search` / `research.query` into `innovation‑scan`** – bring real‑time external data into scans, moving beyond internal LLM knowledge. | Q3 2027 | Market / Technical |
| **Q3 2027 – Review & optimise `weekly‑rollup` & `weekly‑improvement` pipelines** – ensure they run fully, capture metrics, and surface actionable insights. | Q3 2027 | Technical / UX |
| **Q4 2027 – Add monitoring of tool‑usage & skill‑picker correlations** – dashboards that surface which tools are most effective and where picker scores dip. | Q4 2027 | Business / Technical |
| **Q1 2028 – Run full‑system reflection synthesis** – after LLM backend health is restored, re‑run `POST /api/reflection/run` to replace deterministic digests with a complete synthesis. | Q1 2028 | Technical |

\*Quarters are counted from the current quarter (Q4 2026).  

**Rationale drawn from internal reflections**  

- The **employee‑logging gap** and “0 s” durations were repeatedly flagged (2026‑09‑15, 2026‑09‑12, 2026‑09‑07).  
- **`innovation‑scan`** is the fleet bottleneck at ~10 min/run (2026‑10‑03).  
- **Skill‑picker weakness** on `send‑attachment` and `brief‑writing` was noted (2026‑09‑01, 2026‑09‑17).  
- Recommendations to **add low‑frequency, higher‑complexity tasks** and **peer‑delegated work** appear in the “Try next” list (2026‑10‑03).  
- Calls to **review zero‑duration templates**, **enable employee logging**, and **monitor tool usage** are also present (2026‑10‑03).  
- The suggestion to **integrate web‑search/research tools** into `innovation‑scan` (2026‑09‑16, 2026‑09‑10).  

These evidence‑based actions are grouped into the four improvement categories (Technical, UX, Market, Business) and sequenced to address the most critical failures first while building capacity for longer‑term strategic growth.

## Web sources
1. [[JRACLOUD-91572] Option to drill down to the Subtask level in the Timeline (Formerly Roadmap) - Create and track feature requests for Atlassian products.](https://jira.atlassian.com/browse/JSWCLOUD-18677?focusedId=3424755&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel) _(relevance 20, firecrawl)_
2. [How to Create Sub Task Jira: Master Your Workflow](https://www.aakashg.com/create-sub-task-jira/) _(relevance 20, http)_

## Filtered sources _(1 dropped by validator)_
- ~~[Loading https://www.reddit.com/r/jira/comments/t55h7c/what_is_the_easiest_way_to_view_hierarchal/?solution=a29d79b25ef4a046a29d79b25ef4a046&js_challenge=1&jsc_token=2824be10929bdc604753c70a67a1c33129d623f74c0d979ca5715882b5e9eeac&jsc_orig_r=](https://www.reddit.com/r/jira/comments/t55h7c/what_is_the_easiest_way_to_view_hierarchal/)~~ — thin-content (0 chars (min 200))

## Vault hits at time of research
_(none)_
