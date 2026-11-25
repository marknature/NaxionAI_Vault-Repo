---
personaId: "researcher"
taskId: "researcher-brand-scan"
completedAt: "2026-11-25T06:02:49.652Z"
runId: "0765b8fb-9b61-476d-a185-cee7f8797c77"
---

# Brand competitive scan

Completed by researcher.

Naxie · Researcher

Execute searches, then synthesize findings with citations:

1. Search vault for operator's brands: `vault.search({"query": "brand OR company OR product", "limit": 20})`
2. Search for competitive intel: `vault.search({"query": "competitive OR competitor OR landscape", "limit": 20})`
3. Search for operator context: `vault.search({"query": "operator OR business OR startup", "limit": 20})`

Then: Analyze results → Identify key competitors, market positioning, threats/opportunities → Cite specific vault doc IDs → Capture structured findings to `0-Inbox/competitive-landscape-[date].md`
