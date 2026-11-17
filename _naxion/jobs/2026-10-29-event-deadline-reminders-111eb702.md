---
type: job
title: Event deadline reminders
slug: event-deadline-reminders-111eb702
created: 2026-10-29T19:10:11.050Z
jobId: 111eb702-b950-4297-af14-fe02ee981e99
status: succeeded
template: deadline-reminders
persona: naxie
personaName: Naxie
startedAt: 2026-10-29T18:54:14.722Z
finishedAt: 2026-10-29T19:10:11.050Z
---

# Event deadline reminders

- **Status:** succeeded
- **Template:** deadline-reminders
- **Started:** 2026-10-29T18:54:14.722Z
- **Finished:** 2026-10-29T19:10:11.050Z
- **Title:** Event deadline reminders

## Inputs
```json
{
  "chatId": "8767926406"
}
```

### Steps
1. ✓ Read deadline tracker — `pipeline` (0.0s)
2. ✓ Post reminders — `pipeline` (1.2s)

## Answer
⏰ **Event deadlines approaching**

🔴 **Build With AI: Basics** — tomorrow (2026-10-30): https://learn-ai-basics.devpost.com/
🔴 **PayPal AI Hackathon** — tomorrow (2026-10-30): https://paypalaihackathon.devpost.com/
🔴 **Qloo Agentic Hackathon** — tomorrow (2026-10-30): https://qloo.devpost.com/

_3 reminders from the tracked events scan_

<details><summary>Log</summary>

```
[2026-10-29T18:54:14.722Z] Queued — 2 tasks ahead (cap 2 running at once).
[2026-10-29T19:10:09.885Z] Started after 955s in the task queue.
[2026-10-29T19:10:11.049Z] Posted 3 deadline reminder(s) to Telegram chat 8767926406.
```
</details>
