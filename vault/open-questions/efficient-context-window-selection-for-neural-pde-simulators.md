---
created_at: '2026-03-29T18:57:39Z'
source_papers:
- '[[openalex-2603.25025-system-anchored-knee-estimation-for-low-cost-context-window]]'
title: Efficient Context Window Selection
---

**Background:** Autoregressive neural PDE simulators predict future states based on a fixed-length history of past states, where the length of this history is a critical, yet often unoptimized, hyperparameter.

**Question / Future Work:** Can the performance-critical context window length for a given autoregressive neural PDE simulator be identified efficiently without the computational cost of an exhaustive search over all possible window lengths?

**Why It Matters:** The cost of exhaustive context-window tuning can be prohibitively high due to the computational expense of training and evaluating separate models for each candidate window length in PDE forecasting.

**Evidence:** can we identify the performance-critical window for a given autoregressive neural simulator without paying the cost of exhaustive search?