# Lessons learned from daily reflections

Auto-generated from `_neuroworks/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-08-21

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NEUROWORKS_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

## 2026-08-17

### Went wrong
- No failures recorded in window.
- No tool runs, employee activity, or delegations to evaluate.

### Try next
- Add real work to the window: schedule at least one non-reflection task to generate tool/employee data.
- If employees are intended to be active, verify cron/scheduler is triggering them — 0 employees on clock is abnormal for an operational fleet.
- Keep `reflection:daily` as the only guaranteed task; consider retiring it if it’s the sole output.
