---
# CSL-compatible fields
title: "MP-MoE: Matrix Profile-Guided Mixture of Experts for Precipitation Forecasting"
author:
  - literal: "Huyen Ngoc Tran"
  - literal: "Dung Trung Tran"
  - literal: "Hồng Phúc Nguyễn"
  - literal: "Xuan Vu Phan"
  - literal: "Nam-Phong Nguyen"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25046"

# Custom fields
paper_id: "2603.25046"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "post-processing"
  - "loss functions"
  - "rainfall"
  - "convective instability"
architectures:
  - "Mixture of Experts (MoE)"
datasets:
  []
concept_slugs:
  - "mp-moe"
  - "matrix-profile-objective-function"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:22Z"
created_at: "2026-03-29T18:58:22Z"
---

# MP-MoE: Matrix Profile-Guided Mixture of Experts for Precipitation Forecasting

**Authors**: Huyen Ngoc Tran, Dung Trung Tran, Hồng Phúc Nguyễn, Xuan Vu Phan, Nam-Phong Nguyen
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25046](https://arxiv.org/abs/2603.25046)

## Summary

This paper introduces the Matrix Profile-guided Mixture of Experts (MP-MoE) framework to improve precipitation forecasting accuracy, particularly addressing the phase shift sensitivity of conventional point-wise loss functions common in tropical regions. MP-MoE integrates a structural-aware Matrix Profile objective with intensity loss to ensure experts are selected based on subsequence-level similarity rather than just point errors. Evaluating on rainfall data from Vietnamese river basins across various horizons (up to 48 hours), the method significantly outperformed baselines in detecting heavy rainfall events (CSI-M) and reducing temporal misalignment errors (DTW). The work successfully shows that incorporating subsequence structural awareness into MoE selection improves morphological integrity in complex weather predictions.

## Key Contributions

- Proposed MP-MoE, a novel framework combining Matrix Profile-guided structural loss with a Mixture of Experts approach for precipitation post-processing.
- Introduced a structural-aware Matrix Profile objective to mitigate the "double penalty" effect from phase shifts in time series forecasting.
- Demonstrated superior performance over baseline learning methods in heavy rainfall event identification, measured by CSI-M.
- Significantly reduced Dynamic Time Warping (DTW) values, indicating better preservation of the morphological integrity of storm events.

## Limitations

The evaluation is specifically focused on precipitation forecasting in tropical regions (Vietnam), and generalization to other climate regimes is not explicitly tested.

## Open Questions & Future Work

- [[adaptive-tuning-of-mp-moe-hyperparameters]]
- [[extending-mp-moe-to-spatiotemporal-domain]]
- [[online-learning-for-gating-network-adaptation]]

## Key Concepts

- [[mp-moe]]: A probabilistic forecasting framework that uses Matrix Profile similarity to guide the selection of experts within a Mixture of Experts setup.
- [[matrix-profile-objective-function]]: A custom objective function for time series that leverages the Matrix Profile to measure structural similarity between predicted and true subsequences, penalizing phase shifts less severely than point-wise methods.

## Archivist Review

Two novel concepts were approved: the MP-MoE framework itself and the structural Matrix Profile objective function that guides it, as both represent reusable methodological advances over standard point-wise loss and expert selection. Three explicit, well-defined open questions were approved, focusing on adaptive tuning, spatiotemporal extension, and online adaptation, all addressing key limitations in operationalizing structural forecasting methods. No datasets were approved as the mentioned data is specific to a regional study and lacks broad benchmark status.

### Approved Concepts
- Matrix Profile-Guided Mixture of Experts (MP-MoE): It is the central novel framework combining MoE with Matrix Profile loss for improved structural awareness in forecasting.
- Matrix Profile Objective Function: It replaces standard point-wise loss functions with a structural-aware objective based on subsequence similarity, directly addressing the 'double penalty' issue.

### Approved Open Questions
- Adaptive hyperparameter tuning for MP-MoE: Adaptive tuning of loss balance and temporal shift windows is crucial for maintaining optimal trade-offs between shape fidelity and magnitude accuracy as meteorological dynamics change.
- Extending MP-MoE to spatiotemporal domain: Extending to the spatiotemporal domain is necessary to move beyond basin-scale accuracy and ensure physically coherent forecasts across a geographical region.
- Online learning for gating network adaptation: Online learning is critical for maintaining model relevance and predictive power as long-term climate statistics and weather patterns evolve.

### Rejected Candidates
- [dataset] Vietnam river basin rainfall datasets (`vietnam-river-basin-rainfall-datasets`) - paper_local: The dataset is named specifically for a regional study and is not established as a widely reusable benchmark for general time-series research.

## Links

- [Abstract](https://arxiv.org/abs/2603.25046)
- [PDF](https://arxiv.org/pdf/2603.25046)

