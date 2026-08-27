# Lessons learned from daily reflections

Auto-generated from `_neuroworks/reflections/*.md`. Each daily reflection's *What went wrong* and *What to try next* bullets land here. The governance loader prepends this file to every agent system prompt, so yesterday's findings become today's hard rules.

**Rule for the agent reading this:** treat every bullet under *Went wrong* as a known failure mode to avoid this turn. Treat every bullet under *Try next* as a preferred next-step pattern for similar tasks.

---

## 2026-08-26

### Try next
- Check the LLM backend (OpenRouter/OpenAI/Anthropic/Ollama): a hung or very slow provider call, not a code fault, drove the timeout. Raise `NEUROWORKS_REFLECTION_SYNTH_TIMEOUT_MS` only if legitimate synthesis is being cut short.

## 2026-08-25

### Went wrong
- There were no failures or errors recorded during the given time window.

### Try next
- Increase the workload to test the system's scalability and performance under heavier loads.
- Consider integrating more tools and templates to expand the system's capabilities and provide more opportunities for testing and evaluation.
- Review the system's configuration to ensure that employee records and peer attributions are being properly recorded and utilized.
