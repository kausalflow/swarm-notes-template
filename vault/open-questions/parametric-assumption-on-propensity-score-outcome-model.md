---
created_at: '2026-03-29T18:57:12Z'
source_papers:
- '[[openalex-2603.25010-bayesian-propensity-score-augmented-latent-factor-models-for]]'
title: Flexible propensity score outcome modeling
---

**Background:** Causal inference methods often rely on correctly specifying the functional form linking covariates to potential outcomes or treatment assignment. Potential outcomes models incorporating propensity scores rely on a prespecified functional form to incorporate this information.

**Question / Future Work:** Investigate methods to allow the functional form relating the propensity score to the potential outcomes model to be more flexible or non-parametric, especially when using propensity score stratification thresholds that might be mis-specified.

**Why It Matters:** Mis-specification of the functional form or stratification thresholds in propensity score analysis leads directly to biased treatment effect estimates, which is a core concern for the practical utility of the proposed method.

**Evidence:** First, although the propensity score–augmented specification allows for heterogeneous effects across propensity score strata, it still relies on parametric assumptions for both the treatment assignment and outcome models. In particular, because the effect of the propensity score in the outcome model is assumed to follow a prespecified functional form, mis-specification, such as incorrect thresholds used for propensity score stratification, may lead to biased treatment effect estimates.