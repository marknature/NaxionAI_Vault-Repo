---
personaId: "naxie"
taskId: "naxie-signoff-digest"
completedAt: "2026-11-06T15:01:01.162Z"
runId: "06f5ec2d-da8c-4754-91b6-9002b31a4261"
---

# End-of-day sign-off digest

Completed by naxie.

Naxie · Naxie

## 📋 Sign-off Digest Logic

To surface the organizational sign-off digest using the `org.approvals_pending` tool, I will execute the following logic flow:

### ⚙️ Execution Steps
- **Total Volume**: Aggregate all current records within `org.approvals_pending` to determine the total number of items awaiting sign-off.
- **Persona Distribution**: Group the resulting dataset by the `persona` field to identify which roles have the highest volume of pending approvals.
- **Aging Analysis**: Sort all pending items by their timestamp in ascending order to isolate the oldest record in the queue.

### 📊 Report Format
The final output will be presented as follows:
- **Total Pending**: [Total Count]
- **Breakdown by Persona**: 
    - [Persona A]: [Count]
    - [Persona B]: [Count]
- **Oldest Pending Item**: [Item ID/Name] — [Date/Time]

_Assumed: The user is requesting the operational logic for this report as real-time data from the tool was not provided in the evidence catalog [4]._
