---
# CSL-compatible fields
title: "Revealing the influence of participant failures on model quality in cross-silo Federated Learning"
author:
  - literal: "Fabian Stricker"
  - literal: "David Bermbach"
  - literal: "Christian Zirpins"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25289"

# Custom fields
paper_id: "2603.25289"
paper_source: "openalex"
domain: "machine-learning"
tags:
  - "federated learning"
  - "distributed systems"
  - "model_robustness"
  - "model evaluation"
architectures:
  []
datasets:
  []
concept_slugs:
  - "participant-failure-impact-analysis-fl"
  - "model-utility-for-missing-participants"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:59:43Z"
created_at: "2026-03-29T18:59:43Z"
---

# Revealing the influence of participant failures on model quality in cross-silo Federated Learning

**Authors**: Fabian Stricker, David Bermbach, Christian Zirpins
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25289](https://arxiv.org/abs/2603.25289)

## Summary

This paper systematically investigates the reliability gap in Federated Learning (FL) by quantifying the impact of missing participants on model quality across image, tabular, and time-series data. The authors analyze how factors such as data skewness, varying participant availability patterns, and different model architectures modulate this impact. A key finding is that data skewness has a strong influence, potentially causing overly optimistic model evaluations when participant dropouts occur. Furthermore, the study examines the utility of the resulting global model specifically for the participants who were absent during the training process.

## Key Contributions

- Conducted the first systematic study on the impact of missing participants (failures) on model quality in cross-silo Federated Learning.
- Analyzed the influence of factors like data skewness, availability patterns, and model architectures on performance degradation due to participant absence.
- Demonstrated that data skewness significantly impacts model evaluation, potentially leading to overly optimistic assessments when failures are present.
- Investigated the specific utility of the derived global model when evaluated against the data of the participants who were missing during training.

## Limitations

The study focuses specifically on 'missing participants' (crash failures) and may not fully generalize to other fault scenarios like Byzantine attacks or network partitions.

## Open Questions & Future Work

- [[data-agnostic-contribution-metrics-for-fl-failure-prediction]]
- [[concurrent-participant-failure-impact-analysis]]
- [[multivariate-fim-interaction-modeling]]

## Key Concepts

- [[participant-failure-impact-analysis-fl]]: Systematic investigation into how the absence of participants during training rounds affects the final model quality and utility in cross-silo Federated Learning systems.
- [[model-utility-for-missing-participants]]: Assessing the performance and utility of the final global Federated Learning model specifically on the data belonging to participants who experienced failures during training.

## Archivist Review

Archivist review kept only candidates judged central to the paper and reusable across future work. Approved 2 concept(s), 3 open question(s), and 0 dataset(s), with 0 rejected candidate note(s).

### Approved Concepts
- Participant Failure Impact Analysis in FL: This paper systematically studies the previously under-explored impact of participant failures (missing clients) on model quality in Federated Learning, which is critical for production deployment reliability.
- Model Utility for Missing Participants: It addresses a crucial, application-specific metric in FL: whether the resulting global model is still useful or fair to the participants who failed to contribute to the final training round.

### Approved Open Questions
- Data-agnostic impact prediction: Developing data-agnostic, low-overhead contribution metrics is crucial for real-time, practical fault detection and response in FL systems where data privacy prohibits centralized data access for validation.
- Concurrent failure impact analysis: Understanding concurrent failures is necessary for designing robust fault-tolerance mechanisms that account for correlated failure modes common in large-world distributed systems.
- Multivariate FIM interaction modeling: Most real-world failures are multivariate; establishing predictive models that account for modifier interaction is essential for accurate failure prognosis.

## Links

- [Abstract](https://arxiv.org/abs/2603.25289)
- [PDF](https://arxiv.org/pdf/2603.25289)

