---
# CSL-compatible fields
title: "Modeling and Forecasting Tail Risk Spillovers: A Component-Based CAViaR Approach"
author:
  - literal: "Demetrio Lacava"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25217"

# Custom fields
paper_id: "2603.25217"
paper_source: "openalex"
domain: "finance"
tags:
  - "financial-time-series"
  - "risk-management"
  - "quantile-regression"
  - "conditional-heteroskedasticity"
architectures:
  []
datasets:
  []
concept_slugs:
  - "caviar-se"
  - "tail-risk-spillover-component"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:44Z"
created_at: "2026-03-29T18:57:44Z"
---

# Modeling and Forecasting Tail Risk Spillovers: A Component-Based CAViaR Approach

**Authors**: Demetrio Lacava
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25217](https://arxiv.org/abs/2603.25217)

## Summary

This paper introduces CAViaR-SE, a novel extension of the Conditional Autoregressive Value at Risk (CAViaR) model designed to forecast tail risk spillovers. The model decomposes the conditional Value at Risk into a proper-risk component and a spillover component, where the latter is a linear combination of influential assets' tail risks identified via a recursive partial correlation algorithm. The spillover term functions as a predictable quantile shifter, directly modeling the dynamics of the conditional quantile rather than volatility. Empirical results on Dow Jones Industrial Average stocks confirm that CAViaR-SE significantly enhances out-of-sample tail risk forecasts and produces well-calibrated risk measures compared to existing CAViaR variants.

## Key Contributions

- Proposed the Component-Based CAViaR with Spillover Effects (CAViaR-SE) model, which separates conditional VaR into inherent risk and a spillover component driven by external assets' tail risks.
- Introduced a recursive partial correlation algorithm for selecting multiple influential spillover sources with minimal parameterization.
- Demonstrated that spillover effects constitute a substantial portion of total tail risk in the observed financial data.
- Empirical validation showed CAViaR-SE significantly improves out-of-sample tail risk forecasts and provides statistically superior, well-calibrated risk measures compared to standard CAViaR models based on MCS analysis.

## Limitations

The paper focuses exclusively on equity returns (Dow Jones Industrial Average stocks), and its applicability to other asset classes or macroeconomic time series is not tested.

## Open Questions & Future Work

- [[caviar-se-spillover-persistence-zero]]

## Key Concepts

- [[caviar-se]]: An extension of the CAViaR model that decomposes conditional Value at Risk into an inherent risk term and a spillover term driven by influential assets.
- [[tail-risk-spillover-component]]: A predictable quantile shifter in the CAViaR-SE model that captures the influence of tail risks from other assets on the target asset's conditional quantile.

## Archivist Review

Two core concepts were approved: the main CAViaR-SE model as the primary methodological contribution, and the Tail Risk Spillover Component as a reusable abstract mechanism for quantile dynamics. One open question concerning the empirical finding of near-zero autoregression in the spillover term was also retained as it points to an important unresolved dynamic interpretation issue. The selection algorithm was rejected as being a local implementation detail supporting the core concept.

### Approved Concepts
- Component-Based CAViaR with Spillover Effects (CAViaR-SE): It is the novel core methodological contribution of the paper, decomposing VaR into risk and spillover components.
- Tail Risk Spillover Component: This component explicitly models the dependence structure of tail events across different assets, which is a key focus of modern financial risk management.

### Approved Open Questions
- CAViaR Spillover Component Persistence: The finding that $\\hat{\\varphi}_1 \\approx 0$ suggests that the spillover component is driven almost entirely by the exogenous proxy rather than its own persistence, leading to a reallocation of persistence to the proper risk component, which warrants further theoretical and empirical investigation regarding the nature of the spillover dynamics.

### Rejected Candidates
- [concept] Recursive Partial Correlation Algorithm (`recursive-partial-correlation`) - subcomponent_of_broader_mechanism: While the selection method is novel for this context, it is a supporting mechanism for the main CAViaR-SE innovation, making the latter the primary concept.

## Links

- [Abstract](https://arxiv.org/abs/2603.25217)
- [PDF](https://arxiv.org/pdf/2603.25217)

