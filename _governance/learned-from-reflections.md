# Lessons learned from daily reflections

Auto-generated from `_naxion/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-11-24

### Went wrong
- 1 failure: insights:general-task aborted after 8075s with "server received SIGINT" — likely host restart or OOM kill during a long-running job

### Try next
- Log employee/persona attribution if multi-agent routing is intended — currently invisible
- Enable auto-retry (max 1) for operations templates to absorb transient host restarts
- Consider splitting world-ai-news and daily-briefing into parallel sub-pipelines to cut the 185s/132s pipeline serial chains
- Add a watchdog/timeout on general-task (e.g., max 30min) so SIGINT doesn't leave a 2h zombie

## 2026-11-23

### Went wrong
- One `general-task` (insights:general-task) ran for 7.2 hours (25,878s) — extreme outlier vs next slowest at 192s
- No employees recorded on the clock; all work appears to be template-driven only

### Try next
- Investigate the 7.2h `general-task` — check if it hung on an LLM call, looped, or processed an unexpectedly large payload
- Add timeout/guardrails to `general-task` template (e.g., max 30min) to prevent runaway runs
- Consider splitting long-running pipeline chains into smaller steps or async jobs to improve observability
- Enable employee tracking if human-in-the-loop work is expected but not showing up

## 2026-11-22

### Went wrong
- One "evening-recap" task was aborted.

### Try next
- Investigate why the "evening-recap" task is aborting.
- Optimize the "evening-recap" task to reduce its average duration.

## 2026-11-21

### Went wrong
- No tasks failed or were rejected.

### Try next
- No immediate changes are needed as all tasks succeeded and the job performance is within expected ranges.

## 2026-11-20

### Went wrong
- No failures, slow templates, or weak skill picks recorded — quiet night.

### Try next
- Re-run `POST /api/reflection/run` once the LLM backend is healthy to replace this deterministic digest with a full synthesis.

## 2026-11-19

### Went wrong
- No tasks failed.

### Try next
- Optimize the pipeline to reduce its average duration.
- Investigate why daily-briefing is consistently slow.

## 2026-11-18

### Went wrong
- No issues reported.

### Try next
- Consider optimizing the pipeline job 6144bb5a, which is consistently slow.
- Investigate the slow jobs 70d7508c and c057cae4 to ensure they are not causing delays.

## 2026-11-17

### Went wrong
- Peer.review step failed once, all other steps succeeded.

### Try next
- Investigate and optimize the Peer.review step.
- Monitor and potentially reduce idle time during pipeline jobs.

## 2026-11-16

### Try next
- Consider reducing the frequency or scope of the "pipeline" task to ensure it doesn't run unnecessarily.
- Investigate why the "africa-ai-news" task is taking so long and optimize its performance.

## 2026-11-15

### Went wrong
- `board:md-weekly` averaged 1637.6s over 1 run(s) — over the 600s perf budget.
- `events-competition-scan` averaged 609.5s over 1 run(s) — over the 600s perf budget.

### Try next
- Split `board:md-weekly` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~27 min/run.

## 2026-11-14

### Went wrong
- "tool:peer.review step failed 1/1 runs" — 1x (templates: general-task)

### Try next
- Investigate why "pipeline" and "security.scan" are running very quickly, especially if they are not expected to be synchronous.
- Ensure peer reviews are scheduled and run regularly.

## 2026-11-13

### Went wrong
- No issues detected.

### Try next
- Investigate why the "security.scan" tool is consistently zero duration.
- Optimize the "pipeline" tool to reduce its average duration.
- Consider reducing the frequency or disabling the "peer.review" tool if it is not providing value.

## 2026-11-12

### Try next
- Consider running the peer review tool more frequently to ensure it doesn't fail again.
- Optimize the evening-recap task to reduce its average duration.
- Investigate why the peer review tool failed once.

## 2026-11-11

### Try next
- Investigate why some tasks are taking so long, especially the ones lasting over 1000 seconds.
- Optimize the longest tasks to reduce their duration.
- Consider using a different template or tool for the tasks that are taking the most time.

## 2026-11-10

### Went wrong
- 1 instance of "aborted: server received SIGINT" in template "general-task".

### Try next
- Consider optimizing pipeline jobs to reduce their average duration.
- Investigate why "general-task" is failing.

## 2026-11-09

### Went wrong
- No failures reported.

### Try next
- Optimize "peer.review" and "integration.gmail.read" templates.
- Investigate why "research.deep" and "pipeline" steps are consistently slow.

## 2026-11-08

### Try next
- Consider optimizing or parallelizing the pipeline job to reduce its duration.
- Investigate why job cdc6e34a is consistently taking a long time.

## 2026-11-07

### Went wrong
- Nothing went wrong.

### Try next
- Investigate the `evening-recap` pipeline to see if the 163s duration is due to a large data window or a bottleneck in the prompt.
- Audit the `weekly-rollup` and `weekly-improvement` templates to ensure they are actually performing work, as 0s duration suggests they may be returning cached or empty results.

## 2026-11-06

### Went wrong
- `events-competition-scan` experienced extreme latency, taking 18,279.2s (approx. 5 hours) to complete.

### Try next
- Review the `todo-brief` and `evening-recap` templates; avg durations of 0s and 0.2s suggest they may be returning cached or empty results.
- Implement a timeout or pagination limit on the competition scan tool to prevent pipeline hangs.
- Investigate the `events-competition-scan` template to identify why it requires 5+ hours to run.

## 2026-11-05

### Try next
- Analyze the 36s pipeline spikes in job `e6494dcd` to see if a specific news source is causing latency.
- Consolidate `africa-ai-news` and `africa-tech-alerts` into a single persona/template to reduce redundant pipeline calls.

## 2026-11-04

### Try next
- Introduce a peer-review delegation step for `africa-ai-news` to test system resilience under load.
- Since the current fleet is operating at 100% success with low volume, increase the frequency of `innovation-scan` to capture more data.

## 2026-11-03

### Try next
- No changes are necessary as all tasks completed successfully and efficiently.

## 2026-11-02

### Went wrong
- No failures recorded.

### Try next
- Review the 0s duration flows to ensure they are performing intended logic and not skipping necessary steps.
- Investigate job `00fb4a82` (africa-tech-alerts) to determine why its pipeline steps are taking 31-39s, significantly higher than the 14.8s average.

## 2026-11-01

### Try next
- Review `flow:bd01d559` and `flow:7bc13716` (avg 0.1s) to ensure they are performing intended logic and not skipping steps.
- Consolidate the three separate news operations (`world-ai-news`, `africa-ai-news`, `africa-tech-alerts`) into a single regional news aggregator flow to reduce pipeline overhead.

## 2026-10-31

### Try next
- Audit the `pipeline` tool usage in job `ef293a76` to see if the 53s latency can be reduced via parallelization.
- Consolidate the 8 unique `flow:xxxx` templates into named, reusable templates to improve system maintainability.

## 2026-10-30

### Went wrong
- No tasks encountered any failures.

### Try next
- No specific changes are needed as all tasks completed successfully and quickly.

## 2026-10-29

### Try next
- Investigate why events-competition-scan is consistently slow and consider whether it can be optimized or simplified.
- Optimize the africa-ai-news and world-ai-news tasks to reduce their average duration.

## 2026-10-28

### Try next
- Investigate if there are any specific tasks or steps that consistently take longer than usual.
- Consider optimizing the pipeline to potentially reduce the average duration.

## 2026-10-27

### Try next
- Optimize the innovation scan task if it is a network or LLM call, as near-zero average durations are expected for these types of tasks.
- Investigate why the innovation scan task is consistently taking around 120 seconds.
