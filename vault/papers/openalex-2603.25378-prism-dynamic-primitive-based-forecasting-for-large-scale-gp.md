---
# CSL-compatible fields
title: "PRISM: Dynamic Primitive-Based Forecasting for Large-Scale GPU Cluster Workloads"
author:
  - literal: "Xin Wu"
  - literal: "Fei Teng"
  - literal: "Xingwang Li"
  - literal: "Bin Zheng"
  - literal: "Qiang Duan"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25378"

# Custom fields
paper_id: "2603.25378"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "resource-management"
  - "compositional-models"
  - "workload-characterization"
architectures:
  []
datasets:
  []
concept_slugs:
  - "prism-primitive-based-forecasting"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:51Z"
created_at: "2026-03-29T18:57:51Z"
---

# PRISM: Dynamic Primitive-Based Forecasting for Large-Scale GPU Cluster Workloads

**Authors**: Xin Wu, Fei Teng, Xingwang Li, Bin Zheng, Qiang Duan
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25378](https://arxiv.org/abs/2603.25378)

## Summary

The paper addresses the challenge of accurately forecasting volatile, multi-periodic GPU cluster workloads for efficient resource management. The authors introduce PRISM, a novel compositional forecasting framework that employs dictionary-driven temporal decomposition alongside adaptive spectral refinement to capture stable, interpretable workload signatures. Evaluation on large-scale production traces demonstrates that PRISM achieves state-of-the-art performance, particularly in reducing critical burst-phase errors. This methodology offers a robust foundation for architecture-aware dynamic resource allocation in modern AI infrastructure.

## Key Contributions

- Proposed PRISM, a primitive-based compositional forecasting framework for volatile GPU workloads.
- Developed a dual representation by combining dictionary-driven temporal decomposition with adaptive spectral refinement to extract stable workload signatures.
- Achieved state-of-the-art results on large-scale production traces, specifically reducing burst-phase errors.
- Provided an architecture-aware foundation for dynamic resource management in GPU-powered AI platforms.

## Limitations

The abstract does not specify the exact nature or source of the "large-scale production traces" or detail explicit architectural weaknesses.

## Open Questions & Future Work

- [[semantic-meaning-of-learned-primitives]]
- [[alternative-frequency-domain-refinement]]

## Key Concepts

- [[prism-primitive-based-forecasting]]: A primitive-based compositional forecasting framework that combines dictionary-driven temporal decomposition with adaptive spectral refinement.

## Archivist Review

The core contribution is the PRISM framework, which is approved as a reusable concept due to its novel compositional approach combining decomposition and spectral methods for complex time series. Two substantial open questions were identified regarding the semantic interpretability of the learned primitives and potential alternatives for the spectral refinement module, as these point to important future research directions in explainable and advanced time-series modeling. No named datasets were provided, only general production traces, thus no datasets were approved.

### Approved Concepts
- PRISM (Primitive-Based Forecasting): It is the core proposed method for handling complex GPU workload forecasting.

### Approved Open Questions
- Semantics of Learned Workload Primitives: Understanding the learned semantics of the primitives is key to fully realizing the 'interpretable' aspect of the model and ensuring its practical deployment for deriving actionable system insights beyond just predictive accuracy.
- Alternative Spectral Refinement Techniques: While the current spectral refinement is highly effective, exploring alternative frequency-domain modeling techniques could unlock further architectural improvements or reveal fundamental trade-offs between multiplicative weighting and more complex learned transformations for spectral feature extraction.

### Rejected Candidates
- [concept] GPU Cluster Workload Forecasting (`gpu-cluster-workload-forecasting`) - generic: This is the general problem domain, not a specific reusable technique or component introduced by the paper.
- [concept] Dictionary-Driven Temporal Decomposition (`dictionary-driven-temporal-decomposition`) - subcomponent_of_broader_mechanism: This is a component/methodology that supports the main PRISM concept; PRISM itself is the central, reusable contribution.
- [concept] Adaptive Spectral Refinement (`adaptive-spectral-refinement`) - subcomponent_of_broader_mechanism: This is a component/methodology that supports the main PRISM concept; PRISM itself is the central, reusable contribution.
- [concept] Burst-Phase Error Reduction (`burst-phase-error-reduction`) - low_impact: This is a specific performance outcome, not a reusable technical mechanism.

## Links

- [Abstract](https://arxiv.org/abs/2603.25378)
- [PDF](https://arxiv.org/pdf/2603.25378)

