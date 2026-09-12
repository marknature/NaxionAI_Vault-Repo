---
title: NeuroWorks platform — what it is
tags: [neuroworks, clawbot, platform, reference]
---

# NeuroWorks — the platform

**NeuroWorks ("The AI Workforce")** is RUBIEM's private, local AI-agent
platform powered by **clawbot**. It runs on the user's own machine (loopback,
bound to 127.0.0.1) — not a cloud SaaS, and **not** the Natus/Xltek EEG product
of the same name.

## What it does

- **Chat** — a single-persona assistant that plans and executes tasks using a
  catalog of tools (vault search/read, web research, GitHub, file access, doc
  extraction, note capture). Plan → execute (parallel sub-agents) → synthesize
  → QA gate.
- **Team dispatch** — fan a shared brief out to multiple personas in parallel,
  each returning their slice. Pre-organized teams (Product squad, Launch &
  marketing, Insurance desk, Research & GTM) and reusable team templates let a
  user dispatch a whole workflow at once.
- **Personas** — 20+ role-based employees (Product Manager, Software Engineer,
  QA, Designer, DevOps, Marketing, Researcher, Data Analyst, Financial Analyst,
  Contracts Reviewer, Customer Success, Account Executive, Insurance Sales/
  Underwriter, Head of AI, and "Kit" the any-persona adapter). A persona router
  auto-assigns the best specialist to a task.
- **Scheduled tasks** — run templates on a friendly day-of-week + time cadence.
- **Email bridge** — clawbot has a mailbox; users email it ([team]/[chat]
  subject routing), it runs the request and replies with a formatted report.
- **Knowledge vault (second brain)** — a local Obsidian-style markdown vault
  (MiniSearch-indexed) that clawbot reads, searches, and writes captures to.
- **Governance** — admin policy/identity docs that become guardrails prepended
  to every model call.
- **Quality grading** — a deliverable-aware grader (research / creative /
  procedural / code) scoring factuality, citations, and persona fit.
- **Multi-clawbot** — a primary plus peer worker(s); work fans out across them.

## Architecture (high level)

- **Server:** Express + TypeScript (port 7471).
- **Web UI:** Vite + React (port 7470).
- **LLMs:** local **Ollama** (qwen2.5:3b default, qwen2.5-coder:7b, qwen3:4b)
  with optional **OpenRouter** acceleration for planning/synthesis.
- **Vault:** local markdown, git-backed, committed via a debounced queue.

## Status

Active internal development. Recent work: deliverable-aware quality grader,
the email bridge, pre-organized teams + team templates, scheduled tasks, and a
governance guardrail system. (For current specifics, check recent vault notes
and `_neuroworks/reflections/` rather than assuming.)

> When asked for a "status report on NeuroWorks", this platform is the subject
> — never the Natus/EEG product.

