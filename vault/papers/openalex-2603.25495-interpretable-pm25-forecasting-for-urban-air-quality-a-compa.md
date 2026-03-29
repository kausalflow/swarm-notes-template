---
# CSL-compatible fields
title: "Interpretable PM2.5 Forecasting for Urban Air Quality: A Comparative Study of Operational Time-Series Models"
author:
  - literal: "Moazzam Umer Gondal"
  - literal: "Hamad ul Qudous"
  - literal: "Asma Ahmad Farhan"
  - literal: "Sultan Alamri"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25495"

# Custom fields
paper_id: "2603.25495"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "interpretability"
  - "time-series analysis"
  - "model-selection"
  - "model-correction"
architectures:
  []
datasets:
  []
concept_slugs:
  - "online-residual-correction-time-series"
  - "leakage-aware-forecasting-workflow"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:06Z"
created_at: "2026-03-29T18:57:06Z"
---

# Interpretable PM2.5 Forecasting for Urban Air Quality: A Comparative Study of Operational Time-Series Models

**Authors**: Moazzam Umer Gondal, Hamad ul Qudous, Asma Ahmad Farhan, Sultan Alamri
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25495](https://arxiv.org/abs/2603.25495)

## Summary

This study compares lightweight, interpretable time-series models (SARIMAX, Facebook Prophet, NeuralProphet) against each other for short-term PM2.5 forecasting in Beijing, utilizing a leakage-aware workflow and evaluating performance under walk-forward refitting and frozen deployment regimes with online residual correction. Results indicate that Prophet and SARIMAX achieve strong performance, particularly when residual correction is applied to the frozen SARIMAX model, yielding the lowest error (MAE 32.50). The findings advocate for simple additive forecasting strategies due to their competitive accuracy, high interpretability, and significant computational efficiency gains in operational air quality management.

## Key Contributions

- Demonstrated that lightweight additive models (SARIMAX, Prophet) can achieve competitive short-term PM2.5 forecasting accuracy compared to complex, data-intensive models in an urban air quality context.
- Evaluated two operational adaptation regimes: weekly walk-forward refitting and frozen forecasting with online residual correction, showing the latter can significantly reduce computation time.
- Identified that corrected SARIMAX achieved the lowest overall error (MAE 32.50) under the frozen-model regime using online residual correction, surpassing the accuracy of the fully retrained Facebook Prophet model.
- Showed that online residual correction can bring the accuracy of a computationally efficient frozen Facebook Prophet model nearly to its walk-forward counterpart while drastically cutting runtime (from over 15 minutes to under one minute).

## Limitations

The performance of NeuralProphet was consistently less accurate and less stable across both evaluated regimes, suggesting potential limitations for this specific dataset or model setup compared to simpler additive models.

## Open Questions & Future Work

- [[lightweight-hybrid-models-for-regime-change]]
- [[extend-lightweight-adaptation-to-new-cities]]

## Key Concepts

- [[online-residual-correction-time-series]]: A technique used to dynamically adjust the predictions of a time-series model that has been fixed (frozen) in time by using the current forecast error to correct subsequent predictions.
- [[leakage-aware-forecasting-workflow]]: A structured methodology for time-series forecasting that strictly enforces chronological separation of data during training, preprocessing, and feature selection to avoid lookahead bias.

## Archivist Review

The analysis proposed two strong, reusable concepts: the specific deployment strategy of Online Residual Correction and the methodology of a Leakage-Aware Forecasting Workflow. These capture novel contributions regarding operational deployment and evaluation hygiene. Two open questions were approved as they focus on extending adaptation methods to new regimes and generalizing the adaptation strategy, which are central to making lightweight models practical. Other concepts were rejected as they are standard statistical/ML models (SARIMAX, Prophet). The dataset was rejected as it is a location-specific data bucket rather than a standard named benchmark dataset.

### Approved Concepts
- Online Residual Correction (Time Series): It is a specific technique applied to frozen models to adapt them to concept drift in real-time forecasting, which directly impacted the final error metrics in this study.
- Leakage-Aware Forecasting Workflow: The paper explicitly develops and employs this specific workflow combining multiple steps to prevent data leakage, a crucial aspect of robust time-series evaluation.

### Approved Open Questions
- Integrate lightweight hybrid techniques: This is crucial for making lightweight models viable in dynamic environments where pollution sources or meteorological patterns shift, which is common in urban air quality studies.
- Extend adaptation to new environments: Validating the framework across diverse cities and sensing conditions is necessary to confirm its practical utility beyond the single case study of Beijing.

### Rejected Candidates
- [concept] Facebook Prophet (`facebook-prophet`) - not_novel: Facebook Prophet is a widely known, established model and not a novel concept introduced by this paper.
- [concept] SARIMAX (`sarimax`) - not_novel: SARIMAX is a standard statistical modeling technique and not a novel concept from this paper.
- [concept] NeuralProphet (`neuralprophet`) - not_novel: NeuralProphet is an existing established model, not a novel concept introduced by this paper.
- [concept] Frozen Forecasting Regime (`frozen-forecasting-regime`) - paper_local: This is an operational deployment choice evaluated against walk-forward, not a novel reusable forecasting mechanism itself.
- [concept] Walk-Forward Refitting (`walk-forward-refitting`) - not_novel: Walk-forward refitting is a standard, well-known evaluation/deployment procedure, not a novel concept.
- [dataset] Beijing, China (for PM2.5) (`beijing-china-pm25-data`) - low_impact: The dataset label is too generic (location-based) and the focus is on the comparison methodology, not the dataset itself as a reusable benchmark.
- [open_question] Explore federated learning schemes (`explore-federated-learning-for-generalization`) - low_impact: While relevant to generalization, federated learning is a general ML technique, and the question is insufficiently focused on a specific time-series or air-quality mechanism bottleneck compared to the approved candidates.

## Links

- [Abstract](https://arxiv.org/abs/2603.25495)
- [PDF](https://arxiv.org/pdf/2603.25495)

