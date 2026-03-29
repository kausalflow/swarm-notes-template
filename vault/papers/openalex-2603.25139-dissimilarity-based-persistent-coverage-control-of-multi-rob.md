---
# CSL-compatible fields
title: "Dissimilarity-Based Persistent Coverage Control of Multi-Robot Systems for Improving Solar Irradiance Prediction Accuracy in Solar Thermal Power Plants"
author:
  - literal: "Haruki Kawase"
  - literal: "Taiga Sugawara"
  - literal: "A. Daniel Carnerero"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25139"

# Custom fields
paper_id: "2603.25139"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "control systems"
  - "spatial statistics"
  - "sensor networks"
architectures:
  []
datasets:
  []
concept_slugs:
  - "dissimilarity-map-kriging"
  - "persistent-coverage-control-sensor-placement"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:32Z"
created_at: "2026-03-29T18:58:32Z"
---

# Dissimilarity-Based Persistent Coverage Control of Multi-Robot Systems for Improving Solar Irradiance Prediction Accuracy in Solar Thermal Power Plants

**Authors**: Haruki Kawase, Taiga Sugawara, A. Daniel Carnerero
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25139](https://arxiv.org/abs/2603.25139)

## Summary

This paper addresses the challenge of optimizing mobile sensor placement for real-time solar irradiance forecasting in solar thermal power plants, a task where traditional kriging methods lack dynamic sampling strategies. The authors introduce a novel dissimilarity map derived from a kriging model to quantify regions requiring new observations to maximize prediction improvement. They pair this map with a persistent coverage control algorithm designed to guide mobile robots efficiently to these high-value locations. Experimental results using mobile robots across emulated irradiance fields demonstrate that this integrated dissimilarity-based control yields more accurate forecasts compared to established baseline approaches.

## Key Contributions

- Development of a dissimilarity map derived from a kriging model to quantify the value of new sensor observations for solar irradiance prediction.
- Proposal of a persistent coverage control algorithm that uses the dissimilarity map to dynamically guide mobile sensors to optimal data collection locations.
- Demonstration via experiments that the proposed integrated approach achieves more accurate solar irradiance predictions than baseline methods using a minimal number of mobile sensors.

## Limitations

The evaluation was conducted under various *emulated* irradiance fields, suggesting a need for validation in real-world, non-emulated operational environments.

## Open Questions & Future Work

- [[generalization-of-dissimilarity-control-to-dynamic-factors]]

## Key Concepts

- [[dissimilarity-map-kriging]]: A map derived from a kriging model that quantifies the uncertainty or potential for improvement in a spatial prediction field.
- [[persistent-coverage-control-sensor-placement]]: An algorithm for continuously deploying mobile sensors to locations that are predicted to yield the highest marginal improvement in the accuracy of a spatial prediction model.

## Archivist Review

Two core concepts were approved: the 'Dissimilarity Map for Kriging' as a reusable uncertainty metric for active sensing, and the 'Persistent Coverage Control for Sensor Placement' which utilizes this metric to guide agents. The analysis correctly identified a lack of real-world validation under dynamic noise as a key future direction, leading to the approval of one open question concerning the generalization of the control strategy. Datasets were correctly rejected as the evaluation used a non-standard, emulated setup.

### Approved Concepts
- Dissimilarity Map for Kriging: This map is the core mechanism used to drive the sensor placement strategy, quantifying where new measurements will have the highest impact on reducing prediction error.
- Persistent Coverage Control for Sensor Placement: This specific control algorithm ties the dynamic placement of mobile agents directly to the uncertainty metric (the dissimilarity map) to optimize prediction accuracy in real-time.

### Approved Open Questions
- Generalizing Dissimilarity Control: Understanding how to incorporate dynamic, real-world sensor characteristics or complex spatial models into the dissimilarity-based control framework is essential for practical deployment.

### Rejected Candidates
- [dataset] emulated irradiance fields (`emulated-irradiance-fields`) - paper_local: This refers to a specific, non-canonical experimental setup rather than a standardized, reusable benchmark dataset.

## Links

- [Abstract](https://arxiv.org/abs/2603.25139)
- [PDF](https://arxiv.org/pdf/2603.25139)

