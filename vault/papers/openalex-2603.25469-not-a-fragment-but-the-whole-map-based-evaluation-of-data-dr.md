---
# CSL-compatible fields
title: "Not a fragment, but the whole: Map-based evaluation of data-driven Fire Danger Index models"
author:
  - literal: "Shahbaz Alvi"
  - literal: "Italo Epicoco"
  - literal: "José María Costa-Saura"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25469"

# Custom fields
paper_id: "2603.25469"
paper_source: "openalex"
domain: "machine-learning"
tags:
  - "evaluation-methodology"
  - "classification"
  - "ensemble-methods"
architectures:
  []
datasets:
  []
concept_slugs:
  - "map-based-fdi-evaluation"
  - "operational-false-positive-reduction"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:37Z"
created_at: "2026-03-29T18:58:37Z"
---

# Not a fragment, but the whole: Map-based evaluation of data-driven Fire Danger Index models

**Authors**: Shahbaz Alvi, Italo Epicoco, José María Costa-Saura
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25469](https://arxiv.org/abs/2603.25469)

## Summary

This paper addresses the limitations of standard machine learning evaluation metrics for operational Fire Danger Index (FDI) models, which often fail to capture real-world utility, especially concerning false positive rates. The authors propose a novel, map-based evaluation methodology explicitly aligned with decision-making processes in forestry and emergency response. The work systematically evaluates how well models predict fire activity while rigorously quantifying and minimizing false alarms. Finally, it shows that employing an ensemble of ML models enhances both fire identification accuracy and the reduction of false positives.

## Key Contributions

- Proposed a novel map-based evaluation method for Fire Danger Index (FDI) models designed to align with real-world operational decision-making, moving beyond standard classifier metrics.
- Systematically assessed model performance focusing on the accurate identification of fire activity while explicitly accounting for and minimizing false positive rates (false alarms).
- Demonstrated that an ensemble of machine learning models can simultaneously improve fire identification accuracy and reduce the critical operational issue of false positives.

## Limitations

The abstract does not explicitly detail limitations, but the focus on map-based evaluation suggests potential dependence on high-resolution, geographically complete data.

## Key Concepts

- [[map-based-fdi-evaluation]]: A novel evaluation methodology for forest fire forecasting models that incorporates spatial information and operational decision-making alignment, focusing on false positive rates.
- [[operational-false-positive-reduction]]: Focusing on minimizing false alarms in Fire Danger Index models to improve operational utility and decision-making reliability.

## Archivist Review

I approved two concepts as they represent distinct, reusable methodological contributions: a spatial/operational evaluation paradigm and the focus on operational false positive reduction, which is critical for safety-critical ML systems. The proposed open question was too specific to a particular architecture detail (CNN depth) mentioned in the evidence excerpt and thus deemed too paper-local for the vault. The review focused on novelty and reusability in the context of operational ML and evaluation science.

### Approved Concepts
- Map-based Fire Danger Index Evaluation: The paper proposes a novel evaluation method specifically tailored for the operational context of Fire Danger Index (FDI) forecasting, moving beyond standard ML metrics.
- Operational False Positive Reduction in Fire Forecasting: The paper explicitly addresses the critical operational concern of false positives (false alarms) in fire prediction, a common pitfall in safety-critical applications.

### Rejected Candidates
- [open_question] Optimal CNN Depth for False Positive Rejection (`optimal-cnn-depth-for-false-positive-rejection`) - paper_local: The open question is too specific to CNN architectures and the context of this single paper, not representing a broad, recurring research bottleneck.

## Links

- [Abstract](https://arxiv.org/abs/2603.25469)
- [PDF](https://arxiv.org/pdf/2603.25469)

