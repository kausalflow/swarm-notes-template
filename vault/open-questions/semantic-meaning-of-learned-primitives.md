---
created_at: '2026-03-29T18:57:51Z'
source_papers:
- '[[openalex-2603.25378-prism-dynamic-primitive-based-forecasting-for-large-scale-gp]]'
title: Semantics of Learned Workload Primitives
---

**Background:** The PRISM framework decomposes complex, aggregated GPU workload signals into a dynamic mixture of simpler, learnable primitive patterns, drawing an analogy to how an optical prism separates white light into its constituent spectral colors.

**Question / Future Work:** Further investigation is needed into the specific semantic meaning that the learnable primitives ($Q_p$) converge to under different cluster operating conditions (e.g., periods dominated by ML training vs. inference). This includes determining if different sets of primitives emerge when the workload composition shifts drastically (e.g., migration from CPU-heavy workloads to GPU-centric, fine-grained workloads), and assessing the robustness of the decomposition when the diversity-preservation loss ($\\mathcal{L}_{div}$) is relaxed or omitted entirely in such shifts.

**Why It Matters:** Understanding the learned semantics of the primitives is key to fully realizing the 'interpretable' aspect of the model and ensuring its practical deployment for deriving actionable system insights beyond just predictive accuracy.

**Evidence:** By inspecting $\\alpha$, we can transparently identify which primitive dominates the current timeframe, thereby explaining the prediction source (e.g., a spike driven by a burst primitive). This design intentionally decouples the global selection of a primitive ($\\alpha$) from the localized information extraction used to construct it ($A$).