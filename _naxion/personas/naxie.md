---
type: persona-profile
personaId: naxie
personaName: Naxie
generatedAt: 2026-10-08T18:01:34.504Z
factsConsidered: 0
model: gemini-3-flash-preview
---

## What I've learned
* News-scanning tasks (especially super-intelligence) are the primary latency drivers, often exceeding 500s, and require LLM caching or model optimization.
* The workflow pipeline is resilient but opaque; tasks frequently report overall success despite internal failures in `peer.review` and `hermes.delegate`.
* `peer.review` is a current reliability bottleneck with a 50% failure rate, necessitating better input validation or increased timeouts.
* `hermes.delegate` is currently misconfigured for local-only workflows and should be bypassed or retired to reduce template complexity.
* Security checks are intentionally lightweight and synchronous (regex-based), prioritizing sub-millisecond execution over deep analysis.
* The skill-picker struggles with `send-attachment` requests, indicating that skill keywords need refinement to improve matching confidence scores.
