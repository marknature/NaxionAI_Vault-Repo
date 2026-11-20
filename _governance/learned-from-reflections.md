# Lessons learned from daily reflections

Auto-generated from `_naxion/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-11-19

### Went wrong
- No tasks failed.

### Try next
- Investigate why daily-briefing is consistently slow.
- Optimize the pipeline to reduce its average duration.

## 2026-11-18

### Went wrong
- No issues reported.

### Try next
- Investigate the slow jobs 70d7508c and c057cae4 to ensure they are not causing delays.
- Consider optimizing the pipeline job 6144bb5a, which is consistently slow.

## 2026-11-17

### Went wrong
- Peer.review step failed once, all other steps succeeded.

### Try next
- Monitor and potentially reduce idle time during pipeline jobs.
- Investigate and optimize the Peer.review step.

## 2026-11-16

### Went wrong
- No tasks failed or were rejected.

### Try next
- Investigate why the "africa-ai-news" task is taking so long and optimize its performance.
- Consider reducing the frequency or scope of the "pipeline" task to ensure it doesn't run unnecessarily.

## 2026-11-15

### Went wrong
- `events-competition-scan` averaged 609.5s over 1 run(s) — over the 600s perf budget.
- `board:md-weekly` averaged 1637.6s over 1 run(s) — over the 600s perf budget.

### Try next
- Re-run `POST /api/reflection/run` once the LLM backend is healthy to replace this deterministic digest with a full synthesis.
- Split `board:md-weekly` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~27 min/run.

## 2026-11-14

### Went wrong
- "tool:peer.review step failed 1/1 runs" — 1x (templates: general-task)

### Try next
- Ensure peer reviews are scheduled and run regularly.
- Investigate why "pipeline" and "security.scan" are running very quickly, especially if they are not expected to be synchronous.

## 2026-11-13

### Went wrong
- No issues detected.

### Try next
- Consider reducing the frequency or disabling the "peer.review" tool if it is not providing value.
- Optimize the "pipeline" tool to reduce its average duration.
- Investigate why the "security.scan" tool is consistently zero duration.

## 2026-11-12

### Try next
- Investigate why the peer review tool failed once.
- Optimize the evening-recap task to reduce its average duration.
- Consider running the peer review tool more frequently to ensure it doesn't fail again.

## 2026-11-11

### Try next
- Consider using a different template or tool for the tasks that are taking the most time.
- Optimize the longest tasks to reduce their duration.
- Investigate why some tasks are taking so long, especially the ones lasting over 1000 seconds.

## 2026-11-10

### Went wrong
- 1 instance of "aborted: server received SIGINT" in template "general-task".

### Try next
- Investigate why "general-task" is failing.
- Consider optimizing pipeline jobs to reduce their average duration.

## 2026-11-09

### Went wrong
- No failures reported.

### Try next
- Investigate why "research.deep" and "pipeline" steps are consistently slow.
- Optimize "peer.review" and "integration.gmail.read" templates.

## 2026-11-08

### Try next
- Investigate why job cdc6e34a is consistently taking a long time.
- Consider optimizing or parallelizing the pipeline job to reduce its duration.

## 2026-11-07

### Went wrong
- Nothing went wrong.

### Try next
- Audit the `weekly-rollup` and `weekly-improvement` templates to ensure they are actually performing work, as 0s duration suggests they may be returning cached or empty results.
- Investigate the `evening-recap` pipeline to see if the 163s duration is due to a large data window or a bottleneck in the prompt.

## 2026-11-06

### Went wrong
- `events-competition-scan` experienced extreme latency, taking 18,279.2s (approx. 5 hours) to complete.

### Try next
- Investigate the `events-competition-scan` template to identify why it requires 5+ hours to run.
- Implement a timeout or pagination limit on the competition scan tool to prevent pipeline hangs.
- Review the `todo-brief` and `evening-recap` templates; avg durations of 0s and 0.2s suggest they may be returning cached or empty results.

## 2026-11-05

### Try next
- Consolidate `africa-ai-news` and `africa-tech-alerts` into a single persona/template to reduce redundant pipeline calls.
- Analyze the 36s pipeline spikes in job `e6494dcd` to see if a specific news source is causing latency.

## 2026-11-04

### Try next
- Since the current fleet is operating at 100% success with low volume, increase the frequency of `innovation-scan` to capture more data.
- Introduce a peer-review delegation step for `africa-ai-news` to test system resilience under load.

## 2026-11-03

### Try next
- No changes are necessary as all tasks completed successfully and efficiently.

## 2026-11-02

### Went wrong
- No failures recorded.

### Try next
- Investigate job `00fb4a82` (africa-tech-alerts) to determine why its pipeline steps are taking 31-39s, significantly higher than the 14.8s average.
- Review the 0s duration flows to ensure they are performing intended logic and not skipping necessary steps.

## 2026-11-01

### Try next
- Consolidate the three separate news operations (`world-ai-news`, `africa-ai-news`, `africa-tech-alerts`) into a single regional news aggregator flow to reduce pipeline overhead.
- Review `flow:bd01d559` and `flow:7bc13716` (avg 0.1s) to ensure they are performing intended logic and not skipping steps.

## 2026-10-31

### Try next
- Consolidate the 8 unique `flow:xxxx` templates into named, reusable templates to improve system maintainability.
- Audit the `pipeline` tool usage in job `ef293a76` to see if the 53s latency can be reduced via parallelization.

## 2026-10-30

### Went wrong
- No tasks encountered any failures.

### Try next
- No specific changes are needed as all tasks completed successfully and quickly.

## 2026-10-29

### Try next
- Optimize the africa-ai-news and world-ai-news tasks to reduce their average duration.
- Investigate why events-competition-scan is consistently slow and consider whether it can be optimized or simplified.

## 2026-10-28

### Try next
- Consider optimizing the pipeline to potentially reduce the average duration.
- Investigate if there are any specific tasks or steps that consistently take longer than usual.

## 2026-10-27

### Try next
- Investigate why the innovation scan task is consistently taking around 120 seconds.
- Optimize the innovation scan task if it is a network or LLM call, as near-zero average durations are expected for these types of tasks.

## 2026-10-25

### Went wrong
- "events-competition-scan" failed once, resulting in a task abort.

### Try next
- Review and possibly retire any underperforming tools or jobs.
- Optimize "pipeline" jobs to reduce their average duration.
- Investigate why "events-competition-scan" is failing.

## 2026-10-24

### Went wrong
- No issues or failures were observed.

### Try next
- Investigate the single failure in the "peer.review" tool.
- Optimize the "pipeline" tool to reduce its average duration from 448s to a more reasonable value.

## 2026-10-23

### Went wrong
- Slowest steps took up to 28087 seconds.
- 2 out of 4 tasks (africa-ai-news, world-ai-news) failed.

### Try next
- Investigate why the world-ai-news template is failing.
- Optimize the africa-ai-news template.

## 2026-10-22

### Went wrong
- `africa-ai-news` averaged 1924.5s over 2 run(s) — over the 600s perf budget.

### Try next
- Split `africa-ai-news` into parallel sub-agents or trim its heaviest steps — it is the fleet bottleneck at ~32 min/run.

## 2026-10-21

### Try next
- Optimize the 'events-competition-scan' pipeline to reduce its duration.
- Investigate why the 'events-competition-scan' and 'daily-briefing' pipelines are consistently slow.
