---
# CSL-compatible fields
title: "Topological optimization with birth and death cochains"
author:
  - literal: "Thomas Weighill"
  - literal: "Ling Zhou"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25575"

# Custom fields
paper_id: "2603.25575"
paper_source: "openalex"
domain: "other"
tags:
  - "topological data analysis"
  - "optimization"
architectures:
  []
datasets:
  - "arctic ice images"
concept_slugs:
  - "birth-and-death-cochains"
  - "birth-and-death-content-loss"
dataset_slugs:
  - "arctic-ice-images"
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:43Z"
created_at: "2026-03-29T18:58:43Z"
---

# Topological optimization with birth and death cochains

**Authors**: Thomas Weighill, Ling Zhou
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25575](https://arxiv.org/abs/2603.25575)

## Summary

This paper introduces birth and death cochains as unique generalizations of birth and death simplices within persistent cohomology theory. The authors then define birth and death content, derived from these cochains, as generalized persistent times, which are subsequently utilized as novel loss functions for topological optimization. The effectiveness of this approach is validated across diverse data structures, including point clouds, time series, and scalar fields. Finally, the framework is applied to a novel task: topological optimization on a dataset derived from arctic ice images.

## Key Contributions

- Introduction of birth and death cochains as unique generalized counterparts to birth and death simplices in persistent cohomology.
- Definition of birth and death content based on cochains, generalizing birth and death times.
- Demonstration of birth and death content as effective loss functions for topological optimization tasks on point clouds, time series, and scalar fields.
- Novel application of topological optimization using this framework to a dataset of arctic ice images.

## Limitations

The paper focuses on defining the mathematical objects and demonstrating utility on diverse data types, but does not quantify the performance gains against state-of-the-art optimization techniques in detail.

## Open Questions & Future Work

- [[theoretical-stability-of-birth-death-cochains]]

## Key Concepts

- [[birth-and-death-cochains]]: Generalized birth and death elements in persistent cohomology, which are shown to be unique for a given cohomology class.
- [[birth-and-death-content-loss]]: A metric derived from birth and death cochains, generalized from birth/death times, used to formulate loss functions for topological optimization.

## Archivist Review

Two primary concepts related to the mathematical framework—Birth and Death Cochains and the resulting Loss Functions—were approved as they represent the core, reusable mathematical contributions of the paper. One explicit open question regarding the theoretical stability of these new cochains was deemed significant enough for tracking. The named dataset ('arctic ice images') was approved as it grounds a novel application described in the abstract, making it a useful reference point.

### Approved Concepts
- Birth and Death Cochains: This is the core mathematical object introduced, which offers uniqueness for persistent cohomology classes, a property lacking in simplices.
- Birth and Death Content as Loss Functions: This is the central methodological contribution, applying the novel mathematical object directly to drive optimization processes.

### Approved Open Questions
- Theoretical stability of cochains: Establishing theoretical stability bounds for cochains would provide a stronger foundation for their use in optimization compared to the current reliance on empirical observation and heuristic arguments, especially in noisy or clustered data regimes.

### Rejected Candidates
- [dataset] arctic ice images (`arctic ice images`) - other: The specific dataset is approved as it forms the basis of a novel application mentioned in the abstract.

## Datasets

- [[arctic-ice-images]]

## Links

- [Abstract](https://arxiv.org/abs/2603.25575)
- [PDF](https://arxiv.org/pdf/2603.25575)

