# Lessons learned from daily reflections

Auto-generated from `_neuroworks/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-09-01

### Went wrong
- Nothing went wrong.

### Try next
- Check the task ingestion queue to see if incoming jobs are being rejected before reaching the clawbot fleet.
- Trigger a test task using `ollama.generate` to ensure the LLM worker pipeline is still responsive.
- Verify employee schedules; zero active staff suggests a configuration gap or intentional downtime.

## 2026-08-29

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NEUROWORKS_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

## 2026-08-28

### Went wrong
- Nothing went wrong. No execution errors, tool failures, or rejections were recorded.

### Try next
- Profile the `reflection:daily` template execution to see why it required 480.1s with no tool calls or sub-tasks recorded.
- Check workflow schedulers and webhook triggers if automated production jobs were expected to run during this period.

## 2026-08-25

### Went wrong
- There were no failures or errors recorded during the given time window.

### Try next
- Increase the workload to test the system's scalability and performance under heavier loads.
- Consider integrating more tools and templates to expand the system's capabilities and provide more opportunities for testing and evaluation.
- Review the system's configuration to ensure that employee records and peer attributions are being properly recorded and utilized.
