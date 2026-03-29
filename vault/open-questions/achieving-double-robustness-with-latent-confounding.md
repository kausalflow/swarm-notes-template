---
created_at: '2026-03-29T18:57:12Z'
source_papers:
- '[[openalex-2603.25010-bayesian-propensity-score-augmented-latent-factor-models-for]]'
title: Double-robustness with latent factors
---

**Background:** The proposed Bayesian approach for causal inference under latent ignorability requires modeling both the treatment assignment mechanism and the potential outcome model jointly, but uses an approximate Bayesian procedure to avoid model feedback issues by omitting one part of the likelihood during parameter updates.

**Question / Future Work:** Develop a methodology that fully integrates the treatment assignment and outcome models without relying on approximate Bayesian methods or omitting likelihood components, potentially by finding a new way to handle the identification non-uniqueness arising from the scaling ambiguity of latent factors and propensity score parameters.

**Why It Matters:** Achieving double robustness alongside explicitly modeling latent confounding under latent ignorability is a major unresolved goal in causal panel data modeling, as current methods force a trade-off between robustness and explicit modeling of latent confounders.

**Evidence:** Second, because latent factor loadings are estimated from the outcome model and subsequently incorporated into the treatment assignment model, the proposed approach does not fully satisfy the classical double-robustness property: correct specification of either the treatment or outcome model alone is insufficient for consistent estimation. Nevertheless, this dependence reflects the latent ignorability assumption required for identification in the presence of unobserved confounding. Future research aimed at addressing these limitations is worth pursuing.