---
title: Naxie — what it is
tags: [naxie, naxie-agent, platform, reference]
---

# Naxie — the personal assistant

**Naxie** is Mark's private, local AI assistant powered by the **NaxionAI**
engine. It runs on the user's own machine (loopback, bound to 127.0.0.1) —
not a cloud SaaS.

## What it does

- **Chat** — Naxie plans and executes tasks using a catalog of tools (vault
  search/read, web research, GitHub, file access, doc extraction, note
  capture). Plan → execute (parallel sub-agents) → synthesize → QA gate.
- **Team dispatch** — fan a shared brief out to multiple personas in parallel,
  each returning their slice. Pre-organized teams and reusable team templates
  let a user dispatch a whole workflow at once.
- **Personas** — role-based specialists (Software Engineer, IT Support,
  Accountant, Researcher, Social Media Manager, and "Kit" the any-persona
  adapter) led by Naxie. A persona router auto-assigns the best specialist
  to a task.
- **Scheduled tasks** — run templates on a friendly day-of-week + time cadence.
- **Email bridge** — Naxie has a mailbox; users email it ([team]/[chat]
  subject routing), it runs the request and replies with a formatted report.
- **Knowledge vault (second brain)** — a local Obsidian-style markdown vault
  (MiniSearch-indexed) that Naxie reads, searches, and writes captures to.
- **Governance** — admin policy/identity docs that become guardrails prepended
  to every model call.
- **Quality grading** — a deliverable-aware grader (research / creative /
  procedural / code) scoring factuality, citations, and persona fit.
- **Peer workers** — a primary plus peer worker(s); work fans out across them.

## Architecture (high level)

- **Server:** Express + TypeScript (port 7471).
- **Web UI:** Vite + React (port 7470).
- **LLMs:** local **Ollama** with optional **OpenRouter** acceleration for
  planning/synthesis.
- **Vault:** local markdown, git-backed, committed via a debounced queue.

## Status

Active personal deployment. (For current specifics, check recent vault notes
and `_naxion/reflections/` rather than assuming.)
