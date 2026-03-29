---
created_at: '2026-03-29T18:58:58Z'
source_papers:
- '[[openalex-2603.25530-adaptive-subspace-modeling-with-functional-tucker-decomposit]]'
title: Optimal RKHS design point selection
---

**Background:** The functional modeling of a tensor mode requires selecting a set of design points within the continuous domain, which significantly influences the performance and stability of the resulting kernel-based approximation.

**Question / Future Work:** Developing general, application-independent strategies for optimally selecting the design points (sampling points) within the Reproducing Kernel Hilbert Space (RKHS) framework used in FTD is an important open research direction, as this selection directly impacts model stability and adaptability.

**Why It Matters:** Design point selection is a crucial parameter in RKHS models; deriving general optimization strategies would lead to more robust and universally applicable functional tensor decomposition methods.

**Evidence:** Another important open research question is the design point selection. Although this choice may be application‑dependent or constrained by measurement availability, investigating general strategies for determining optimal sampling points in RKHS models could yield more stable and adaptable methods. Such strategies may even merit consideration during the planning of data acquisition.