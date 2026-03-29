---
# CSL-compatible fields
title: "Bayesian Propensity Score-Augmented Latent Factor Models for Causal Inference with Time-Series Cross-Sectional Data"
author:
  - literal: "Licheng Liu"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25010"

# Custom fields
paper_id: "2603.25010"
paper_source: "openalex"
domain: "time-series"
tags:
  - "causal-inference"
  - "time-series-cross-sectional"
  - "bayesian-methods"
  - "latent-variable-models"
architectures:
  []
datasets:
  []
concept_slugs:
  - "bayesian-propensity-latent-factor-model"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:12Z"
created_at: "2026-03-29T18:57:12Z"
---

# Bayesian Propensity Score-Augmented Latent Factor Models for Causal Inference with Time-Series Cross-Sectional Data

**Authors**: Licheng Liu
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25010](https://arxiv.org/abs/2603.25010)

## Summary

This paper introduces a Bayesian propensity score-augmented latent factor model specifically tailored for causal inference in time-series cross-sectional datasets. The methodology models treatment assignment via latent factor loadings while flexibly incorporating propensity scores (e.g., through stratification) into the outcome model, allowing for richer heterogeneity analysis within treatment comparison strata. To enable estimation, the authors develop an approximate Bayesian procedure designed to circumvent the feedback problem inherent in traditional Bayesian propensity score methods. The approach is shown via simulation and application (examining political connections on firm value) to yield more credible causal effect estimates than current alternatives.

## Key Contributions

- Propose a Bayesian propensity score-augmented latent factor model designed specifically for causal inference on time-series cross-sectional data.
- The framework explicitly models treatment assignment using latent factor loadings and flexibly incorporates the propensity score, such as via stratification, into the outcome model.
- Introduces an approximate Bayesian procedure to estimate the model, specifically addressing the feedback problem common in Bayesian propensity score analyses.
- Demonstrates superior performance in capturing heterogeneity across propensity-score strata compared to existing approaches, leading to more credible causal comparisons.

## Limitations

The paper mentions adopting an *approximate* Bayesian procedure, implying potential limitations related to approximation error, though this is necessary to solve the feedback problem.

## Open Questions & Future Work

- [[parametric-assumption-on-propensity-score-outcome-model]]
- [[achieving-double-robustness-with-latent-confounding]]

## Key Concepts

- [[bayesian-propensity-latent-factor-model]]: A novel causal inference framework that integrates latent factor modeling with propensity score stratification within a Bayesian setting to better handle time-series cross-sectional data.

## Archivist Review

Archivist review kept only candidates judged central to the paper and reusable across future work. Approved 1 concept(s), 2 open question(s), and 0 dataset(s), with 2 rejected candidate note(s).

### Approved Concepts
- Bayesian Propensity Score-Augmented Latent Factor Model: This is the central methodological contribution, combining Bayesian inference, latent factor modeling, and propensity score augmentation specifically for complex time-series panel data causal questions.

### Approved Open Questions
- Flexible propensity score outcome modeling: Mis-specification of the functional form or stratification thresholds in propensity score analysis leads directly to biased treatment effect estimates, which is a core concern for the practical utility of the proposed method.
- Double-robustness with latent factors: Achieving double robustness alongside explicitly modeling latent confounding under latent ignorability is a major unresolved goal in causal panel data modeling, as current methods force a trade-off between robustness and explicit modeling of latent confounders.

### Rejected Candidates
- [concept] Approximate Bayesian Procedure (`approximate-bayesian-procedure`) - subcomponent_of_broader_mechanism: This is an implementation detail for the estimation of the main model, not a reusable, standalone methodological contribution.
- [concept] Model Feedback Problem (`model-feedback-problem`) - paper_local: This is a generic description of an issue common in Bayesian propensity score analysis, not a named, reusable concept introduced by this paper.

## Links

- [Abstract](https://arxiv.org/abs/2603.25010)
- [PDF](https://arxiv.org/pdf/2603.25010)

