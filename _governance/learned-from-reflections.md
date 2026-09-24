# Lessons learned from daily reflections

Auto-generated from `_neuroworks/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-09-23

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NEUROWORKS_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

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

## 2026-09-01

### Try next
- Verify employee schedules; zero active staff suggests a configuration gap or intentional downtime.
- Trigger a test task using `ollama.generate` to ensure the LLM worker pipeline is still responsive.
- Check the task ingestion queue to see if incoming jobs are being rejected before reaching the clawbot fleet.

## 2026-08-28

### Went wrong
- Nothing went wrong. No execution errors, tool failures, or rejections were recorded.

### Try next
- Check workflow schedulers and webhook triggers if automated production jobs were expected to run during this period.
- Profile the `reflection:daily` template execution to see why it required 480.1s with no tool calls or sub-tasks recorded.

## 2026-08-25

### Went wrong
- There were no failures or errors recorded during the given time window.

### Try next
- Review the system's configuration to ensure that employee records and peer attributions are being properly recorded and utilized.
- Consider integrating more tools and templates to expand the system's capabilities and provide more opportunities for testing and evaluation.
- Increase the workload to test the system's scalability and performance under heavier loads.
