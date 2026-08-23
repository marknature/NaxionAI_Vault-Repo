---
title: "Naxie Improvement Plan — Knowledge, Efficiency, UX"
created: 2026-08-23
tags: [naxie, improvement, triage]
owner: Nature
---

# Naxie Improvement — Knowledge, Efficiency, UX

**Goal:** Improve Naxie's capabilities as a Personal Assistant to Nature by enhancing knowledge, efficiency, and user experience.

## Steps

### 1. Knowledge Expansion — due 2026-10-04 (6 weeks)
- Owner: Research team (Researcher persona)
- Action: Assign team of researchers to update database with latest environmental conservation, sustainability, eco-friendly practices.
- Deliverable: >=500 new vault entries, sourced, cited [vault:2-Permanent/...], via research.multiperspective + vault.write
- Tool: research.deep + omnisignal.publish

### 2. AI Model Refining — due 2026-11-23 (3 months)
- Owner: AI Engineers (Model Router)
- Action: Fine-tune language processing — Gemini/Nvidia active provider tuning, prompt alignment >95%, reduce errors via quality.check + human.request gate
- Deliverable: Response accuracy >95% in user testing (quality.check persona_fit >0.95)
- Tool: model-providers + llm.generate + quality.check

### 3. User Interface Enhancement — due 2026-10-23 (2 months)
- Owner: Dani (Product Designer) + Naxie
- Action: Intuitive visual/interactive elements on /naxie — HUD orb, KnowledgeGraph, push-to-talk, Telegram HTML rendering
- Deliverable: Ship, user satisfaction >=80% survey
- Tool: web/src/pages/Naxie.tsx

### 4. Specialist Network Development — due 2027-05-23 (9 months)
- Owner: Naxie (triage) + Riley (Recruiter)
- Action: Establish 20+ verified environmental experts, n8n-triggered delegation, 90%+ response rate
- Deliverable: 20 experts in vault/org chart, delegated via n8n.trigger_webhook / specialist network
- Tool: n8n.* + personas + org.reports

## Risks & Mitigations
- Data quality/quantity → gate via confidence scoring + HITL review
- Model bias/errors → quality.check + governance.check, monitor factuality_risk <0.4
- UI alienation → A/B, 80% satisfaction gate before full rollout
- Specialist partnerships → early outreach, Riley pipeline

## Definition of Done (all gates equal model-providers small/large split)
1. >=500 new environmental entries in vault [vault:2-Permanent/...]
2. Accuracy >95% (quality.check)
3. UI redesign shipped, satisfaction >=80%
4. >=20 verified experts, response rate >=90%

## Telegram Rendering
- Now HTML: **bold**, *italic*, `code`, ```pre```, [link](url) → Telegram <b>/<i>/<code>/<pre>/<a> via markdownToTelegramHtml in telegram-bridge.ts:135
