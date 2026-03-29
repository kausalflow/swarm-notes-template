---
created_at: '2026-03-29T18:58:43Z'
source_papers:
- '[[openalex-2603.25575-topological-optimization-with-birth-and-death-cochains]]'
title: Theoretical stability of cochains
---

**Background:** The stability of birth and death simplices used in topological optimization can be low because they are highly localized and can be altered by small perturbations in the data.

**Question / Future Work:** Investigate theoretical guarantees for the stability of $\\epsilon$-birth and $\\epsilon$-death cochains, as the authors currently only provide a heuristic argument for their increased practical stability over simplices when filtration values cluster.

**Why It Matters:** Establishing theoretical stability bounds for cochains would provide a stronger foundation for their use in optimization compared to the current reliance on empirical observation and heuristic arguments, especially in noisy or clustered data regimes.

**Evidence:** While we have good reason not to expect a theoretical guarantee of stability for $\\epsilon$-birth and $\\epsilon$-death cochains, we have a heuristic argument for why they may be more stable than birth and death simplices in practice (see Section 6).