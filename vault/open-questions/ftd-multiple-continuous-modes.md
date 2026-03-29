---
created_at: '2026-03-29T18:58:58Z'
source_papers:
- '[[openalex-2603.25530-adaptive-subspace-modeling-with-functional-tucker-decomposit]]'
title: Expand FTD to multiple continuous modes
---

**Background:** The Functional Tucker Decomposition (FTD) formulation, as presented, is computationally restricted to models possessing only one continuous mode due to specific constraints in solving for the core tensor within the alternating optimization scheme.

**Question / Future Work:** Expanding the Functional Tucker Decomposition (FTD) to handle scenarios involving multiple continuous modes, which is relevant for complex data like multi-channel medical signals (e.g., ECG or EEG data), requires overcoming the current computational limitations associated with core tensor optimization in such higher-order continuous factorizations.

**Why It Matters:** Extending FTD to multiple continuous modes would broaden its applicability to more complex, multi-channel time-series data prevalent in fields like medical signal processing, directly addressing a stated technical bottleneck.

**Evidence:** For instance, the current formulation is restricted to one continuous mode because of computational considerations regarding the solution for the core tensor. Even though this setup already covers many real-world applications, an expansion to an FTD with multiple continuous modes could be interesting for medical challenges such as the analysis of electrocardiogram (ECG) or electroencephalogram (EEG) data with multiple channels.