# Lessons learned from daily reflections

Auto-generated from `_naxion/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-10-09

### Went wrong
- 7 unique flow templates (e.g., `flow:d3e13193`, `flow:503c883f`) reported 0s average duration, indicating potential no-ops or skipped logic.
- `vault.read` failed 1/1 runs during the `naxie:converse` template.

### Try next
- Consolidate repetitive flow IDs into named templates to reduce fragmentation.
- Audit the 7 flow templates with 0s duration to determine if they are performing actual work or should be retired.
- Debug `vault.read` permissions or pathing specifically for the `naxie:converse` persona.

## 2026-10-08

### Went wrong
- "tool:github.get_file step failed 1/1 runs" — 1x (templates: general-task).

### Try next
- Investigate tool `github.get_file`: 1/1 step runs failed — check its error output before the next scheduled run.
- Re-run `POST /api/reflection/run` once the LLM backend is healthy to replace this deterministic digest with a full synthesis.

## 2026-10-07

### Went wrong
- Despite step failures, the overall tasks still succeeded, indicating hidden retries or fallback paths that add latency and complexity.
- hermes.delegate failed its sole execution (100% failure rate) in the general‑task template.
- peer.review failed 1 of 2 executions (50% failure rate), affecting the daily‑briefing and general‑task templates.

### Try next
- Review the skill‑picker for send‑attachment; the weak keyword match (score 15) suggests a better‑matched skill could reduce unnecessary attachment handling.
- Consider replacing the placeholder security.scan with an actual scanner if real security checks are required, otherwise keep the current fast implementation.
- Add result caching for frequent pipeline calls (e.g., news‑scan templates) to cut the avg 95.6 s duration.
- Improve peer.review reliability: adjust its input validation or increase timeout to eliminate the 50% failure rate.
- Investigate and fix hermes.delegate configuration or retire the template if delegation is unnecessary.

## 2026-10-06

### Went wrong
- No tasks failed or were rejected; there were no errors to report.

### Try next
- Profile the pipeline substeps for jobs a732cc97, 69041923, and b77069d9 to pinpoint operations >250 s and replace them with pre‑compiled regex or cached results.
- Cut innovation-scan frequency from three runs per day to two (morning and evening) to reduce pipeline load by roughly one‑third while preserving coverage.
- Merge africa‑ai‑news, world‑ai‑news, and super‑intelligence‑news into a single parameterized news‑briefing tool that takes a region/topic flag, lowering template maintenance overhead.
- Retain the current security.scan configuration; its 0 s average is correct and indicates no unnecessary I/O.

## 2026-10-05

### Went wrong
- Skill picker weak on `research-deep`: avg score 15 (keyword-only) over 1 run(s).
- Skill picker weak on `brief-writing`: avg score 15 (keyword-only) over 1 run(s).
- "tool:vault.read step failed 1/2 runs" — 1x (templates: general-task).

### Try next
- Enrich the `brief-writing` skill metadata (intent phrases) so the picker stops matching on keywords alone.
- Investigate tool `vault.read`: 1/2 step runs failed — check its error output before the next scheduled run.

## 2026-10-03

### Went wrong
- No failures or rejections to report.
- Nothing went wrong; all tasks were completed successfully without any failures or rejections.
- `innovation-scan` averaged 621.5s over 4 run(s) — over the 600s perf budget.
- No failures or errors recorded; nothing went wrong

### Try next
- Add a low‑frequency, higher‑complexity task (e.g., a quarterly strategy scan) to diversify workload.
- Introduce at least one peer‑delegated task to test load‑balancing across the fleet.
- Review the zero‑duration templates to confirm they are performing intended actions.
- Enable employee logging to track who runs which tasks.
- Review the automation process to ensure that employee involvement is correctly logged when necessary.
- Consider monitoring tool usage and skill picker correlations to better understand system interactions and improve task efficiency.
- Investigate the weekly-rollup and weekly-improvement tasks to ensure they are functioning as intended and not skipping necessary steps.
- Split `innovation-scan` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~10 min/run.
- Add a lightweight validation step to todo-brief, weekly-rollup, and weekly-improvement to confirm they are performing intended work (e.g., check output length > 0)
- Consider batching innovation-scan runs or increasing its timeout to avoid potential stalls if duration trends upward
- Schedule system-audit during off‑peak hours to reduce impact on other local tasks
- Review the insights:board-meeting template to see if its 84 s average can be trimmed by caching reusable data sources

## 2026-10-02

### Went wrong
- No failures, slow templates, or weak skill picks recorded — quiet night.

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
