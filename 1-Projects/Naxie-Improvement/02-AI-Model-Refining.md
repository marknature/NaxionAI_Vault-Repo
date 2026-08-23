---
title: "Naxie Step 2 — AI Model Refining"
parent: "Naxie Improvement"
due: 2026-11-23
owner: AI Engineers (Gemini/Nvidia)
---

# Step 2 — AI Model Refining

**Goal:** >95% accuracy, reduced errors.

## Sub-tasks
- 2.1 Baseline: quality.check on 50 Naxie replies (factuality_risk <0.4, persona_fit >0.5)
- 2.2 Tune GEMINI_SMALL/LARGE + Nvidia fallback chain (model-providers.ts)
- 2.3 Fine-tune prompt: Naxie adaptive systemPromptOverride (already crisp/warm)
- 2.4 Eval: user testing 95%+ accuracy gate

**Toolchain:** model-providers, llm.generate, quality.check, governance.check
**Risk:** biases → monitor factuality_risk, bias eval
