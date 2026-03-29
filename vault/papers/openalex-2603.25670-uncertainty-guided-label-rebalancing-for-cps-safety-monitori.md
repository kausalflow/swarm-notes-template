---
# CSL-compatible fields
title: "Uncertainty-Guided Label Rebalancing for CPS Safety Monitoring"
author:
  - literal: "John Ayotunde"
  - literal: "Qinghua Xu"
  - literal: "Guancheng Wang"
  - literal: "Lionel C. Briand"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25670"

# Custom fields
paper_id: "2603.25670"
paper_source: "openalex"
domain: "time-series"
tags:
  - "imbalance-learning"
  - "safety-critical-systems"
  - "time-series-forecasting"
  - "model-supervised-learning"
architectures:
  []
datasets:
  - "UAV benchmark"
concept_slugs:
  - "u-balance-uncertainty-guided-rebalancing"
  - "uncertainty-guided-label-rebalancing-ulnr"
  - "gatedmlp-uncertainty-predictor"
dataset_slugs:
  - "uav-benchmark"
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T19:00:08Z"
created_at: "2026-03-29T19:00:08Z"
---

# Uncertainty-Guided Label Rebalancing for CPS Safety Monitoring

**Authors**: John Ayotunde, Qinghua Xu, Guancheng Wang, Lionel C. Briand
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25670](https://arxiv.org/abs/2603.25670)

## Summary

This paper addresses extreme class imbalance in Cyber-Physical System (CPS) safety monitoring by proposing U-Balance, a novel supervised approach that incorporates behavioral uncertainty into dataset rebalancing. The framework first employs a GatedMLP-based predictor to estimate the uncertainty score for time-series telemetry windows. The core innovation is the uncertainty-guided label rebalancing (uLNR) mechanism, which probabilistically relabels highly uncertain 'safe' samples as 'unsafe' to augment the minority class with boundary examples. Evaluated on a UAV benchmark with a 46:1 imbalance, U-Balance significantly outperformed baselines, achieving an F1 score of 0.806, confirming the value of exploiting uncertainty information prior to training the final safety predictor.

## Key Contributions

- Proposed U-Balance, a framework leveraging behavioral uncertainty to rebalance highly imbalanced CPS safety monitoring datasets, achieving a 14.3 percentage point F1 improvement over the strongest baseline.
- Introduced the Uncertainty-Guided Label Rebalancing (uLNR) mechanism, which probabilistically relabels uncertain 'safe' samples as 'unsafe' to enrich the minority class without synthesis.
- Developed a GatedMLP-based uncertainty predictor that summarizes telemetry windows into kinematic features to quantify behavioral uncertainty in CPS operations.
- Demonstrated that behavioral uncertainty is moderately correlated with safety outcomes in a large-scale UAV telemetry dataset with a 46:1 imbalance ratio.

## Limitations

The paper notes that the correlation between behavioral uncertainty and safety is only moderate, suggesting that uncertainty alone does not capture all safety-critical nuances. Further research is needed to explore direct fusion methods compared to pre-training rebalancing.

## Open Questions & Future Work

- [[ucas-generalizability-across-cps-domains]]
- [[impact-of-uncertainty-estimator-accuracy-on-rebalancing]]

## Key Concepts

- [[u-balance-uncertainty-guided-rebalancing]]: A supervised framework that uses behavioral uncertainty to guide label rebalancing in extremely imbalanced time-series safety monitoring datasets.
- [[uncertainty-guided-label-rebalancing-ulnr]]: A mechanism that probabilistically flips the label of 'safe' time-series samples exhibiting high behavioral uncertainty to 'unsafe' to enrich the minority class.
- [[gatedmlp-uncertainty-predictor]]: A GatedMLP model used to generate a distributional kinematic feature summary of a time-series window and output a behavioral uncertainty score.

## Archivist Review

Archivist review kept only candidates judged central to the paper and reusable across future work. Approved 3 concept(s), 2 open question(s), and 1 dataset(s), with 1 rejected candidate note(s).

### Approved Concepts
- U-Balance: It is the proposed overall methodology that combines uncertainty prediction and guided relabeling for imbalanced safety monitoring.
- Uncertainty-Guided Label Rebalancing (uLNR): This is the core novel mechanism for class enrichment that exploits uncertainty in otherwise safe data points.
- GatedMLP-based Uncertainty Predictor: This is the specific architectural choice for estimating the 'behavioral uncertainty' required by the overall method.

### Approved Open Questions
- Generalizability across CPS domains: Assessing performance across diverse CPS types is crucial for establishing the broad applicability of data rebalancing techniques that rely on inferred uncertainty signals.
- Impact of uncertainty estimator accuracy: Understanding the relationship between the quality of uncertainty estimation and rebalancing efficacy is key to making the system robust to variations in uncertainty predictor design.

### Rejected Candidates
- [concept] Behavioral Uncertainty (`behavioral-uncertainty`) - subcomponent_of_broader_mechanism: This concept is too broad/vague; the paper operationalizes it via a specific 'GatedMLP-based Uncertainty Predictor' and the 'uLNR' mechanism, which are better suited as reusable concepts.

## Datasets

- [[uav-benchmark]]

## Links

- [Abstract](https://arxiv.org/abs/2603.25670)
- [PDF](https://arxiv.org/pdf/2603.25670)

