---
# CSL-compatible fields
title: "Adaptive Subspace Modeling With Functional Tucker Decomposition"
author:
  - literal: "Noah Steidle"
  - literal: "Joppe De Jonghe"
  - literal: "Mariya Ishteva"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25530"

# Custom fields
paper_id: "2603.25530"
paper_source: "openalex"
domain: "other"
tags:
  - "tensor decomposition"
  - "functional data analysis"
  - "kernel methods"
architectures:
  - "Tucker Decomposition"
datasets:
  []
concept_slugs:
  - "functional-tucker-decomposition-ftd"
  - "rkhs-tensor-modeling"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:58Z"
created_at: "2026-03-29T18:58:58Z"
---

# Adaptive Subspace Modeling With Functional Tucker Decomposition

**Authors**: Noah Steidle, Joppe De Jonghe, Mariya Ishteva
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25530](https://arxiv.org/abs/2603.25530)

## Summary

This paper introduces the Functional Tucker Decomposition (FTD), a novel tensor decomposition technique designed to model multidimensional data originating from continuous processes by embedding mode-wise continuity constraints directly into the tensor structure. The FTD leverages Reproducing Kernel Hilbert Spaces (RKHS) to model these continuous modes adaptively, preserving the multi-linear subspace properties of the Tucker model without requiring a pre-selected basis. This RKHS-driven approach yields expressive factor descriptions suitable for targeted subspace modeling. The authors validate the FTD's utility by demonstrating superior classification performance in domains like hyperspectral imaging and multivariate time series analysis.

## Key Contributions

- Introduction of Functional Tucker Decomposition (FTD) which embeds mode-wise continuity constraints directly into the standard Tucker model.
- Utilization of Reproducing Kernel Hilbert Spaces (RKHS) for modeling continuous modes without needing an a-priori basis selection.
- Demonstration of the FTD's effectiveness in domain-variant tensor classification tasks across hyperspectral imaging and multivariate time series analysis.

## Limitations

The abstract does not explicitly state limitations, but potential limitations may involve computational overhead due to the RKHS machinery or kernel selection sensitivity.

## Open Questions & Future Work

- [[ftd-multiple-continuous-modes]]
- [[optimal-rkhs-design-point-selection]]

## Key Concepts

- [[functional-tucker-decomposition-ftd]]: A novel tensor decomposition method that incorporates mode-wise continuity constraints using reproducing kernel Hilbert spaces.
- [[rkhs-tensor-modeling]]: Using Reproducing Kernel Hilbert Spaces (RKHS) to implicitly learn continuous functions representing modes in tensor decomposition.

## Archivist Review

Two primary novel concepts were approved: the Functional Tucker Decomposition (FTD) as the core method, and the use of RKHS as the enabling mechanism for continuity. Two substantial open questions concerning extending the FTD to multiple continuous modes and optimizing RKHS design points were approved, as they represent critical future research bottlenecks. Generic application domains listed as datasets were rejected as they do not refer to specific, reusable benchmarks.

### Approved Concepts
- Functional Tucker Decomposition (FTD): It is the core novel mathematical framework proposed in the paper, integrating continuous modeling into the standard Tucker structure.
- RKHS-driven Tensor Modeling: It provides the specific mechanism (RKHS) that enables the functional adaptability of the proposed decomposition.

### Approved Open Questions
- Expand FTD to multiple continuous modes: Extending FTD to multiple continuous modes would broaden its applicability to more complex, multi-channel time-series data prevalent in fields like medical signal processing, directly addressing a stated technical bottleneck.
- Optimal RKHS design point selection: Design point selection is a crucial parameter in RKHS models; deriving general optimization strategies would lead to more robust and universally applicable functional tensor decomposition methods.

### Rejected Candidates
- [open_question] Transfer continuity to Tensor Train Decomposition (`transfer-continuity-to-tensor-train-decomposition`) - low_impact: This is a valid future work direction but is an extension rather than an unresolved limitation of the core FTD method itself.
- [dataset] hyperspectral imaging (`hyperspectral-imaging`) - paper_local: This refers to a general class of data, not a specific, named benchmark dataset warranting a standalone note.
- [dataset] multivariate time series analysis (`multivariate-time-series-analysis`) - paper_local: This refers to a general application domain, not a specific, named dataset warranting a standalone note.

## Links

- [Abstract](https://arxiv.org/abs/2603.25530)
- [PDF](https://arxiv.org/pdf/2603.25530)

