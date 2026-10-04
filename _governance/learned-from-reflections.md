# Lessons learned from daily reflections

Auto-generated from `_naxion/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-10-03

### Went wrong
- Nothing went wrong; all tasks were completed successfully without any failures or rejections.

### Try next
- Review the automation process to ensure that employee involvement is correctly logged when necessary.
- Consider monitoring tool usage and skill picker correlations to better understand system interactions and improve task efficiency.
- Investigate the weekly-rollup and weekly-improvement tasks to ensure they are functioning as intended and not skipping necessary steps.

## 2026-10-02

### Went wrong
- No failures, slow templates, or weak skill picks recorded — quiet night.

### Try next
- Re-run `POST /api/reflection/run` once the LLM backend is healthy to replace this deterministic digest with a full synthesis.

## 2026-10-01

### Went wrong
- Skill picker weak on `send-attachment`: avg score 15 (keyword-only) over 2 run(s).
- `daily-briefing` averaged 1355.9s over 2 run(s) — over the 600s perf budget.

### Try next
- Enrich the `send-attachment` skill metadata (intent phrases) so the picker stops matching on keywords alone.
- Split `daily-briefing` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~23 min/run.

## 2026-09-28

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NAXION_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

## 2026-09-20

### Went wrong
- Nothing went wrong. There were 0 failures and 0 rejected tasks.

### Try next
- Investigate the `todo-brief` template to ensure it isn't returning empty results or skipping logic.
- Audit the employee tracking system to determine why no staff were recorded as active during task execution.
- Increase the frequency of `innovation-scan` or `system-audit` to better utilize the fleet during low-volume periods.

## 2026-09-17

### Went wrong
- Skill picker for `brief-writing` returned a weak score of 15 (keyword-only match) for 2 runs, indicating poor alignment between task requirements and employee metadata.
- The `todo-brief` template reported an `avgDurationSec` of 0s. Unlike synchronous scanners, a brief generation typically requires LLM I/O; this suggests the task may have returned a cached result or skipped execution.

### Try next
- Increase task load or schedule additional persona-driven tasks; the current fleet utilization is negligible.
- Update the `brief-writing` skill definition with more descriptive metadata to improve picker confidence scores.
- Audit the `todo-brief` template to ensure it is not failing silently or returning empty strings.

## 2026-09-16

### Went wrong
- Nothing went wrong.

### Try next
- Audit the `todo-brief` template logic to confirm it is actually generating content and not just returning an empty string or cached result.
- Investigate the employee tracking configuration to ensure active clawbots are correctly attributed to the "on the clock" stat.
- Integrate `web.search` or `research.query` into the `innovation-scan` template to move beyond internal data processing.

## 2026-09-15

### Went wrong
- Zero employees were recorded as "on the clock" despite 5 tasks being completed, suggesting a disconnect between task execution and employee session logging.
- The `todo-brief` template recorded a 0s duration. Unlike synchronous scanners, a briefing template should involve processing time; this indicates the task likely exited early or found no data to process.

### Try next
- Assign a `research` or `web` based task to verify if the tool-call logging (currently empty) is actually functional.
- Check the integration between the task runner and the employee time-tracking module to fix the "none recorded" status.
- Audit the `todo-brief` template to ensure it isn't skipping logic; 0s duration is a red flag for a non-security tool.

## 2026-09-12

### Try next
- Increase task load to test system performance beyond single-instance runs.
- Audit the `weekly-rollup` template; 0s duration suggests it may be returning empty results or skipping processing logic.
- Investigate the employee logging system; tasks are executing without being attributed to active staff.

## 2026-09-10

### Try next
- Attach `web.search` or `research.market` tools to the `innovation-scan` template to provide real-time data.
- Verify the employee heartbeat/clock-in mechanism to ensure active users are being tracked during task execution.
- Increase task frequency or batch size to gather statistically significant performance data.

## 2026-09-07

### Try next
- Audit the employee logging configuration to determine why active tasks are not being attributed to "on the clock" staff.
- Increase task volume or trigger frequency for the `innovation-scan` to utilize idle capacity.
- Review the `innovation-scan` template to determine if adding `web.search` or `research.market` tools would improve the scan's depth beyond internal LLM knowledge.

## 2026-09-06

### Try next
- Check employee initialization configs; 0 employees on the clock suggests agents are not being correctly summoned or authenticated.
- Verify task triggers and scheduling, as 0 production tasks were initiated.
