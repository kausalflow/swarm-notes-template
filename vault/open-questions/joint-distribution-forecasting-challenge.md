---
created_at: '2026-03-29T18:57:17Z'
source_papers:
- '[[openalex-2603.25370-a-distribution-to-distribution-neural-probabilistic-forecast]]'
title: Scalable joint distribution parameterization
---

**Background:** Extending neural forecasting frameworks to model the full probability distribution over all state variables remains a technical hurdle in distribution-to-distribution learning.

**Question / Future Work:** The current implementation focuses on modeling marginal predictive distributions for individual state variables rather than the full joint distribution over the complete state vector. Extending the framework to full joint distribution-to-distribution forecasting requires developing scalable parameterizations for high-dimensional dependence structures and covariance representations.

**Why It Matters:** The ability to model the full joint predictive distribution is crucial for accurately capturing cross-variable dependencies and propagating correlated uncertainty in multi-dimensional dynamical systems.

**Evidence:** Extending the framework to full joint distribution-to-distribution forecasting would require scalable parameterisations of high-dimensional dependence structures and covariance representations, which remains a substantial challenge and is beyond the scope of the present work.