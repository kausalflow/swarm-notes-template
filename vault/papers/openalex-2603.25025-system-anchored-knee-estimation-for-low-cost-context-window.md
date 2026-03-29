---
# CSL-compatible fields
title: "System-Anchored Knee Estimation for Low-Cost Context Window Selection in PDE Forecasting"
author:
  - literal: "Wenshuo Wang"
  - literal: "Fan Zhang"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25025"

# Custom fields
paper_id: "2603.25025"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "physics-informed-ml"
  - "model selection"
  - "computational efficiency"
architectures:
  []
datasets:
  []
concept_slugs:
  - "system-anchored-knee-estimation"
  - "knee-aware-selection"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:39Z"
created_at: "2026-03-29T18:57:39Z"
---

# System-Anchored Knee Estimation for Low-Cost Context Window Selection in PDE Forecasting

**Authors**: Wenshuo Wang, Fan Zhang
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25025](https://arxiv.org/abs/2603.25025)

## Summary

This paper addresses the unformalized problem of low-cost context-window selection for autoregressive neural PDE simulators by treating it as an independent algorithmic challenge. The authors introduce System-Anchored Knee Estimation (SAKE), a two-stage method that first identifies a structured candidate set using physically interpretable system anchors. Subsequently, it performs a knee-aware downstream selection within this candidate set to find the optimal context length. Evaluated across eight PDEBench families, SAKE proved to be the strongest overall low-cost selector at a matched budget, achieving strong predictive accuracy while incurring only 5.1% of the search cost of alternative methods. The method effectively optimizes the trade-off between model complexity (context window size) and long-term rollout performance for physical simulations.

## Key Contributions

- Formalized context-window selection for fixed-window autoregressive neural PDE simulators as an independent low-cost algorithmic problem.
- Proposed System-Anchored Knee Estimation (SAKE), a two-stage selector using physical anchors and knee-aware selection.
- Achieved state-of-the-art performance as a matched-budget low-cost selector across all eight PDEBench families.
- Demonstrated significant search-cost savings (94.9\% normalized) compared to other selection methods.

## Limitations

The paper focuses on fixed-window autoregressive simulators, and the applicability to variable-length or non-autoregressive PDE models is not discussed.

## Open Questions & Future Work

- [[efficient-context-window-selection-for-neural-pde-simulators]]

## Key Concepts

- [[system-anchored-knee-estimation]]: A two-stage method for context-window selection in autoregressive neural PDE simulators that identifies a candidate set from system anchors before performing knee-aware downstream selection.
- [[knee-aware-selection]]: A method for selecting the optimal context window size that focuses on the 'knee' point where marginal returns diminish significantly in downstream performance.

## Archivist Review

I approved the main method, System-Anchored Knee Estimation (SAKE), as a central reusable concept for low-cost resource tuning in sequence models. I also approved the underlying optimization principle, Knee-aware Selection, as a generalizable tuning strategy. The open question targets the core problem SAKE solves: efficiently finding the optimal fixed context window for autoregressive time-series/PDE models. I rejected the dataset candidate as PDEBench is a family of benchmarks rather than a single, essential dataset for the vault.

### Approved Concepts
- System-Anchored Knee Estimation (SAKE): It is the central novel method proposed for low-cost context-window selection in neural PDE simulators.
- Knee-aware Downstream Selection: The paper introduces a specific selection criterion (\"knee-aware\") that optimizes for a trade-off point, which is a reusable concept in resource-constrained model tuning.

### Approved Open Questions
- Efficient Context Window Selection: The cost of exhaustive context-window tuning can be prohibitively high due to the computational expense of training and evaluating separate models for each candidate window length in PDE forecasting.

### Rejected Candidates
- [dataset] PDEBench (`pdebench`) - low_impact: PDEBench is a collection of benchmark datasets/families for PDE simulation, not a single canonical dataset worthy of a standalone note.

## Links

- [Abstract](https://arxiv.org/abs/2603.25025)
- [PDF](https://arxiv.org/pdf/2603.25025)

