---
type: research
topic: GenAI-stack whitepaper review (Dr. Srini's reference)
for: final-report Microsoft / enterprise-AI thread
created: 2026-06-01
tags:
  - india-study-abroad
  - research
---

# Whitepaper review — "The Generative AI Stack" (Dr. Srini)

> The reference Dr. Srini shared after our Microsoft chat. **Author = Nikhil Srinivasan** (Senior Lecturer, MIS) — almost certainly "Dr. Srini" himself. April 2026, ~10,900 words, practitioner white paper (not peer-reviewed, but cites Vaswani 2017, Lewis 2020 RAG, Ouyang 2022 RLHF, etc., so defensible to cite).

## The core idea (OSI-style layered model)
**"The model is table stakes, not a differentiator."** Advantage lives in the layers *around* the model. Seven layers (L0–L6):
- L0 compute · L1 foundation models · L2 inference/deployment · **L3 memory & knowledge (RAG, vector DBs, knowledge graphs) ← the "data layer"** · **L4 orchestration/agents** · **L5 context & interaction design** · L6 applications.
- Cross-cutting: safety, evaluation, observability, governance. Failures propagate upward.

## The key nuance for MY essay (upgrades Dr. Srini's takeaway)
- My visit takeaway was: *"companies need to post-train models to their business."* The paper **complicates this productively:**
  - **Fine-tuning = L1** (modifies the model; expensive; redo when base model updates). **Context/prompt engineering = L5** (instant, cheap).
  - Explicit guidance: **"Exhaust prompt and context engineering before committing to fine-tuning."** Fine-tuning *too early* is a named failure mode.
  - ⟶ **Reconciled claim (use this — it's the sophisticated version):** the *intuition* (AI must be adapted to each business) is right, but the *mechanism* is mostly **L3 retrieval + L5 context**, with true post-training reserved for style/vocabulary/format. A reflection essay rewards exactly this kind of "I learned the mechanism is subtler than I first thought."

## Answers the question I asked the weak MS speaker
- My question — *does the enterprise data layer need rebuilding around agents?* — **= L3 in this framework.** L3 is "where your organization's proprietary knowledge meets the AI system... the primary site for data governance." My **"ontology layer"** instinct maps to **L3 knowledge graphs** (entity relationships, not just semantic similarity). Validates the instinct.
- Supporting case: **Microsoft Azure SRE Agent** — *"retrieval quality, not model quality, was the primary determinant of resolution accuracy"* (35,000+ incidents autonomously, Apr 2026). Plus **M365 Copilot** = org-data-as-context. Both are clean **Microsoft-Hyderabad tie-ins.**

## Quote bank (verbatim)
- "The model is table stakes, not a differentiator. The actual competitive moat is built in L3 through L5."
- "Giving the model an open-book exam rather than a closed-book one." (RAG)
- "Exhaust prompt and context engineering before committing to fine-tuning."
- "This layer is also where your organization's proprietary knowledge meets the AI system. That makes it the primary site for data governance decisions." (L3)

## ⚠️ Gaps
- **No India content at all** — this supplies the *enterprise-AI substrate*, not the India angle. Source India framing elsewhere (DVC notes, DPI story).
- Vendor/tool tables are landscape lists — cite the conceptual sections only.

## APA (provisional — confirm before citing)
- Srinivasan, N. (2026). *The generative AI stack: A layered framework for understanding AI technologies* [White paper]. *(Self-published; confirm exact title/availability with Dr. Srini.)*
