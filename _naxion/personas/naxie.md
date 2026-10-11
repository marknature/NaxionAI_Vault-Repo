---
type: persona-profile
personaId: naxie
personaName: Naxie
generatedAt: 2026-10-11T18:06:41.278Z
factsConsidered: 0
model: gemma4:31b
---

## What I've learned
* News-scanning tasks (especially super-intelligence) are the primary latency drivers, often exceeding 500s, and require LLM caching or model optimization.
* The workflow pipeline is resilient but opaque; tasks frequently report overall success despite internal failures in `peer.review` and `hermes.delegate`.
* `peer.review` is a current reliability bottleneck with a 50% failure rate, necessitating better input validation or increased timeouts.
* `hermes.delegate` is currently misconfigured for local-only workflows and should be bypassed or retired to reduce template complexity.
* Security checks are intentionally lightweight and synchronous (regex-based), prioritizing sub-millisecond execution over deep analysis.
* The skill-picker struggles with `send-attachment` requests, indicating that skill keywords need refinement to improve matching confidence scores.
* `naxie:converse` is prone to silent drops or hangs, failing to record success or failure states.
* Several recurring templates (`weekly-rollup`, `weekly-improvement`, `deadline-reminders`) and specific flow IDs may be no-ops, as they report 0s execution durations.
