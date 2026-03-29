---
# CSL-compatible fields
title: "Spatiotemporal System Forecasting with Irregular Time Steps via Masked Autoencoder"
author:
  - literal: "Kewei Zhu"
  - literal: "Yanze Xin"
  - literal: "Jinwei Hu"
  - literal: "Xiaoyuan Cheng"
  - literal: "Yiming Yang"
  - literal: "Sibo Cheng"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25597"

# Custom fields
paper_id: "2603.25597"
paper_source: "openalex"
domain: "time-series"
tags:
  - "time-series-forecasting"
  - "autoencoders"
  - "attention-mechanisms"
  - "spatiotemporal-data"
  - "deep-learning-for-science"
architectures:
  - "Masked Autoencoder"
datasets:
  []
concept_slugs:
  - "physics-spatiotemporal-masked-autoencoder"
  - "irregular-time-step-forecasting"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:33Z"
created_at: "2026-03-29T18:57:33Z"
---

# Spatiotemporal System Forecasting with Irregular Time Steps via Masked Autoencoder

**Authors**: Kewei Zhu, Yanze Xin, Jinwei Hu, Xiaoyuan Cheng, Yiming Yang, Sibo Cheng
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25597](https://arxiv.org/abs/2603.25597)

## Summary

This paper introduces the Physics-Spatiotemporal Masked Autoencoder (P-STMAE) designed to improve prediction accuracy for high-dimensional dynamical systems characterized by irregular observation time steps. The method uniquely combines convolutional autoencoders for spatial feature extraction with masked autoencoders tailored for non-uniform time series, leveraging attention to perform a single-pass reconstruction of the complete physical sequence. By avoiding direct data imputation, the model maintains the physical integrity of the system fields being modeled. Evaluation on simulated and real-world ocean temperature data shows P-STMAE outperforms traditional recurrent and convolutional approaches in terms of accuracy and robustness.

## Key Contributions

- Proposed the Physics-Spatiotemporal Masked Autoencoder to forecast high-dimensional systems with irregular time steps without explicit data imputation.
- Integrated convolutional autoencoders for spatial feature extraction with MAE optimized for time-series reconstruction using attention mechanisms.
- Achieved significant improvements in prediction accuracy and robustness over traditional convolutional and recurrent network methods on simulated and real-world ocean data.
- Demonstrated the ability to capture complex spatiotemporal patterns for applications like climate modeling and fluid dynamics using only input data structure, not explicit physical constraints.

## Limitations

The paper does not explicitly discuss limitations but focuses on simulated and specific real-world ocean data, suggesting domain specificity may be a factor.

## Open Questions & Future Work

- [[improving-positional-encoding-for-irregular-time-series]]
- [[multi-objective-optimization-accuracy-structure]]

## Key Concepts

- [[physics-spatiotemporal-masked-autoencoder]]: A novel method combining convolutional autoencoders for spatial feature extraction and masked autoencoders optimized for irregular time series, using attention to reconstruct the full sequence.
- [[irregular-time-step-forecasting]]: The challenge of accurately modeling and predicting high-dimensional dynamical systems where observations are available at non-uniform or irregular time intervals.

## Archivist Review

Two core concepts were approved: the novel 'Physics-Spatiotemporal Masked Autoencoder' architecture and the underlying problem of 'Irregular Time Step Forecasting', as both are reusable and central to the contribution. Two open questions were selected, focusing on improving temporal encoding specifically for irregular series and resolving the structural fidelity vs. numerical accuracy trade-off, both representing specific, non-boilerplate research directions. Other candidates were rejected for being generic future work or representing standard architectural limitations rather than novel, specific research gaps.

### Approved Concepts
- Physics-Spatiotemporal Masked Autoencoder: This is the novel integrated architecture proposed to handle irregular time series data by combining spatial feature extraction (CNN-like) with time-series reconstruction (MAE-like).
- Irregular Time Step Forecasting: The core problem addressed is forecasting when observations arrive at non-uniform intervals, a common difficulty in real-world scientific data that standard models struggle with.

### Approved Open Questions
- Advanced positional encoding for irregular time steps: The choice of positional encoding directly impacts how well the model understands the sequence timing, which is crucial for irregular time series forecasting accuracy.
- Balancing numerical accuracy and structural fidelity: Resolving this trade-off is key to building models that are both numerically accurate and visually/physically coherent.

### Rejected Candidates
- [open_question] Enhancing Transformer scalability for long sequences (`transformer-quadratic-complexity-scalability`) - generic: This is a generic limitation of the Transformer architecture and not a novel, specific open question arising directly from this masked autoencoder design for irregular time series.
- [open_question] Investigating advanced spatial encoding techniques (`alternatives-to-CAE-for-spatial-encoding`) - low_impact: This is framed as generic future work about replacing a component (CAE) rather than an inherent, unsolved bottleneck in the proposed method itself.
- [open_question] Broad validation on diverse real-world data (`broader-validation-real-world-datasets`) - low_impact: This is boilerplate future work (more experiments on more data) and does not specify a concrete, unresolved technical problem.

## Links

- [Abstract](https://arxiv.org/abs/2603.25597)
- [PDF](https://arxiv.org/pdf/2603.25597)

