# Lessons learned from daily reflections

Auto-generated from `_naxion/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-10-10

### Went wrong
- Multiple templates (`weekly-rollup`, `weekly-improvement`, `deadline-reminders`, and both `flow` IDs) reported 0s average duration, suggesting they may be no-ops or skipping execution logic.
- `naxie:converse` failed to record a success or failure (0 ok, 0 failed), indicating a potential hang or silent drop.

### Try next
- Review the `flow` templates (24c2f50e, f1748896) to verify if 0s execution is expected behavior.
- Audit the `weekly-rollup` and `weekly-improvement` templates to ensure they are actually performing work and not returning empty successes.
- Investigate the `naxie:converse` trigger to determine why it failed to resolve.

## 2026-10-09

### Went wrong
- `vault.read` failed 1/1 runs during the `naxie:converse` template.
- 7 unique flow templates (e.g., `flow:d3e13193`, `flow:503c883f`) reported 0s average duration, indicating potential no-ops or skipped logic.

### Try next
- Debug `vault.read` permissions or pathing specifically for the `naxie:converse` persona.
- Audit the 7 flow templates with 0s duration to determine if they are performing actual work or should be retired.
- Consolidate repetitive flow IDs into named templates to reduce fragmentation.

## 2026-10-08

### Went wrong
- "tool:github.get_file step failed 1/1 runs" — 1x (templates: general-task).

### Try next
- Re-run `POST /api/reflection/run` once the LLM backend is healthy to replace this deterministic digest with a full synthesis.
- Investigate tool `github.get_file`: 1/1 step runs failed — check its error output before the next scheduled run.

## 2026-10-07

### Went wrong
- peer.review failed 1 of 2 executions (50% failure rate), affecting the daily‑briefing and general‑task templates.
- hermes.delegate failed its sole execution (100% failure rate) in the general‑task template.
- Despite step failures, the overall tasks still succeeded, indicating hidden retries or fallback paths that add latency and complexity.

### Try next
- Investigate and fix hermes.delegate configuration or retire the template if delegation is unnecessary.
- Improve peer.review reliability: adjust its input validation or increase timeout to eliminate the 50% failure rate.
- Add result caching for frequent pipeline calls (e.g., news‑scan templates) to cut the avg 95.6 s duration.
- Consider replacing the placeholder security.scan with an actual scanner if real security checks are required, otherwise keep the current fast implementation.
- Review the skill‑picker for send‑attachment; the weak keyword match (score 15) suggests a better‑matched skill could reduce unnecessary attachment handling.

## 2026-10-06

### Went wrong
- No tasks failed or were rejected; there were no errors to report.

### Try next
- Retain the current security.scan configuration; its 0 s average is correct and indicates no unnecessary I/O.
- Merge africa‑ai‑news, world‑ai‑news, and super‑intelligence‑news into a single parameterized news‑briefing tool that takes a region/topic flag, lowering template maintenance overhead.
- Cut innovation-scan frequency from three runs per day to two (morning and evening) to reduce pipeline load by roughly one‑third while preserving coverage.
- Profile the pipeline substeps for jobs a732cc97, 69041923, and b77069d9 to pinpoint operations >250 s and replace them with pre‑compiled regex or cached results.

## 2026-10-05

### Went wrong
- "tool:vault.read step failed 1/2 runs" — 1x (templates: general-task).
- Skill picker weak on `brief-writing`: avg score 15 (keyword-only) over 1 run(s).
- Skill picker weak on `research-deep`: avg score 15 (keyword-only) over 1 run(s).

### Try next
- Investigate tool `vault.read`: 1/2 step runs failed — check its error output before the next scheduled run.
- Enrich the `brief-writing` skill metadata (intent phrases) so the picker stops matching on keywords alone.

## 2026-10-03

### Went wrong
- No failures or errors recorded; nothing went wrong
- `innovation-scan` averaged 621.5s over 4 run(s) — over the 600s perf budget.
- Nothing went wrong; all tasks were completed successfully without any failures or rejections.
- No failures or rejections to report.

### Try next
- Review the insights:board-meeting template to see if its 84 s average can be trimmed by caching reusable data sources
- Schedule system-audit during off‑peak hours to reduce impact on other local tasks
- Consider batching innovation-scan runs or increasing its timeout to avoid potential stalls if duration trends upward
- Add a lightweight validation step to todo-brief, weekly-rollup, and weekly-improvement to confirm they are performing intended work (e.g., check output length > 0)
- Split `innovation-scan` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~10 min/run.
- Investigate the weekly-rollup and weekly-improvement tasks to ensure they are functioning as intended and not skipping necessary steps.
- Consider monitoring tool usage and skill picker correlations to better understand system interactions and improve task efficiency.
- Review the automation process to ensure that employee involvement is correctly logged when necessary.
- Enable employee logging to track who runs which tasks.
- Review the zero‑duration templates to confirm they are performing intended actions.
- Introduce at least one peer‑delegated task to test load‑balancing across the fleet.
- Add a low‑frequency, higher‑complexity task (e.g., a quarterly strategy scan) to diversify workload.

## 2026-10-02

### Went wrong
- No failures, slow templates, or weak skill picks recorded — quiet night.

## 2026-10-01

### Went wrong
- `daily-briefing` averaged 1355.9s over 2 run(s) — over the 600s perf budget.
- Skill picker weak on `send-attachment`: avg score 15 (keyword-only) over 2 run(s).

### Try next
- Split `daily-briefing` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~23 min/run.
- Enrich the `send-attachment` skill metadata (intent phrases) so the picker stops matching on keywords alone.

## 2026-09-28

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NAXION_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

## 2026-09-20

### Went wrong
- Nothing went wrong. There were 0 failures and 0 rejected tasks.

### Try next
- Increase the frequency of `innovation-scan` or `system-audit` to better utilize the fleet during low-volume periods.
- Audit the employee tracking system to determine why no staff were recorded as active during task execution.
- Investigate the `todo-brief` template to ensure it isn't returning empty results or skipping logic.

## 2026-09-17

### Went wrong
- The `todo-brief` template reported an `avgDurationSec` of 0s. Unlike synchronous scanners, a brief generation typically requires LLM I/O; this suggests the task may have returned a cached result or skipped execution.
- Skill picker for `brief-writing` returned a weak score of 15 (keyword-only match) for 2 runs, indicating poor alignment between task requirements and employee metadata.

### Try next
- Audit the `todo-brief` template to ensure it is not failing silently or returning empty strings.
- Update the `brief-writing` skill definition with more descriptive metadata to improve picker confidence scores.
- Increase task load or schedule additional persona-driven tasks; the current fleet utilization is negligible.

## 2026-09-16

### Went wrong
- Nothing went wrong.

### Try next
- Integrate `web.search` or `research.query` into the `innovation-scan` template to move beyond internal data processing.
- Investigate the employee tracking configuration to ensure active clawbots are correctly attributed to the "on the clock" stat.
- Audit the `todo-brief` template logic to confirm it is actually generating content and not just returning an empty string or cached result.

## 2026-09-15

### Went wrong
- The `todo-brief` template recorded a 0s duration. Unlike synchronous scanners, a briefing template should involve processing time; this indicates the task likely exited early or found no data to process.
- Zero employees were recorded as "on the clock" despite 5 tasks being completed, suggesting a disconnect between task execution and employee session logging.

### Try next
- Audit the `todo-brief` template to ensure it isn't skipping logic; 0s duration is a red flag for a non-security tool.
- Check the integration between the task runner and the employee time-tracking module to fix the "none recorded" status.
- Assign a `research` or `web` based task to verify if the tool-call logging (currently empty) is actually functional.

## 2026-09-12

### Try next
- Investigate the employee logging system; tasks are executing without being attributed to active staff.
- Audit the `weekly-rollup` template; 0s duration suggests it may be returning empty results or skipping processing logic.
- Increase task load to test system performance beyond single-instance runs.
