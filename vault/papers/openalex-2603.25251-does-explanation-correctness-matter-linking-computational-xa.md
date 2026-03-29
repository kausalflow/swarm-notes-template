---
# CSL-compatible fields
title: "Does Explanation Correctness Matter? Linking Computational XAI Evaluation to Human Understanding"
author:
  - literal: "Gregor Baer"
  - literal: "chao zhang"
  - literal: "Isel Grau"
  - literal: "Pieter Van Gorp"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25251"

# Custom fields
paper_id: "2603.25251"
paper_source: "openalex"
domain: "nlp"
tags:
  - "explainable-ai"
  - "human-subject-study"
  - "evaluation-methodology"
  - "fidelity"
architectures:
  []
datasets:
  []
concept_slugs:
  - "explanation-correctness-manipulation"
  - "forward-simulation-xai-evaluation"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:59:54Z"
created_at: "2026-03-29T18:59:54Z"
---

# Does Explanation Correctness Matter? Linking Computational XAI Evaluation to Human Understanding

**Authors**: Gregor Baer, chao zhang, Isel Grau, Pieter Van Gorp
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25251](https://arxiv.org/abs/2603.25251)

## Summary

This paper investigates the critical, yet untested, assumption that computational explanation correctness (fidelity) directly translates to better human understanding in Explainable AI (XAI). The authors conducted a user study ($N=200$) on a time series classification task, manipulating explanation correctness at four distinct levels ($100\%$ down to $55\%$) while participants performed forward simulation (predicting the AI's output from the explanation). The results indicate a non-linear relationship: performance significantly drops between $100\%$ and $70\%$ correctness, but further reduction below $70\%$ offers no additional harm, suggesting a threshold effect on human comprehension. Furthermore, the study found that lower correctness primarily reduces the number of participants who learn the decision pattern, and that $100\%$ correctness alone does not guarantee understanding. These findings emphasize the necessity of validating functional XAI metrics against measurable human outcomes.

## Key Contributions

- Demonstrated experimentally that manipulating explanation correctness from 100% down to 70% significantly reduces human understanding (measured by performance), but further degradation below 70% yields no additional performance loss.
- Showed that lower explanation correctness disproportionately affects the *proportion* of participants who learn the decision pattern, rather than uniformly shifting the performance of all participants.
- Established that even 100% functionally correct explanations do not guarantee high human understanding, as only a subset of participants achieved high accuracy in the forward simulation task.
- Found that self-reported ratings only correlate with demonstrated performance when explanations are fully correct and the participant has successfully learned the underlying decision pattern.

## Limitations

The study was conducted using a time series classification task, and the findings might not generalize perfectly to other domains or model types (e.g., vision, NLP). The sample size (N=200) may limit the statistical power of some exploratory analyses.

## Open Questions & Future Work

- [[xai-correctness-granularity-85-100-percent]]
- [[factors-beyond-correctness-for-understanding]]
- [[conditions-for-informative-self-reports]]

## Key Concepts

- [[explanation-correctness-manipulation]]: An experimental manipulation that systematically varies the functional correctness of model explanations provided to human evaluators.
- [[forward-simulation-xai-evaluation]]: A human evaluation protocol where participants predict the model's decision based only on the provided explanation, testing the utility of the explanation for tracing model behavior.

## Archivist Review

Two concepts were approved as they represent reusable, specific methodological contributions: controlling explanation fidelity (Explanation Correctness Manipulation) and the human evaluation task used (Forward Simulation). Two open questions were approved focusing on the non-linear link between correctness and understanding, and factors enabling learning beyond correctness. The remaining candidates were rejected: the dataset was too generic (a task, not a named dataset), and one open question was deemed too specific to the paper's chosen functional metrics. This archive remains focused on core, reusable ML mechanisms and unsolved research bottlenecks.

### Approved Concepts
- Explanation Correctness Manipulation: This is the core methodological contribution, systematically varying the fidelity of the explanation provided to users in a controlled manner.
- Forward Simulation in XAI User Studies: It defines the specific task used to measure human understanding, where users must predict the model's output based solely on the explanation.

### Approved Open Questions
- Finer-Grained Correctness Link: Resolving this gap is critical because if functional improvements in this high-correctness range do not yield corresponding human benefits, resources spent optimizing for these small functional gains may be misallocated.
- Factors Supporting Explanation Learning: Identifying these necessary additional factors is crucial for developing XAI evaluation frameworks that move beyond functional metrics to ensure explanations actually foster comprehension.
- Informative Self-Report Conditions: Determining the contexts where subjective measures reliably align with objective performance is essential for establishing them as valid evaluation instruments, rather than being informative only under ideal circumstances.

### Rejected Candidates
- [dataset] time series classification task (`time series classification task`) - generic: This is a generic task description, not a specific, named, reusable benchmark dataset.
- [open_question] Correctness Metric Equivalence Test (`equivalence-of-correctness-metrics`) - paper_local: This is a localized methodological validation question regarding the specific metrics used in this paper, rather than a broader, generalizable open problem for XAI research.

## Links

- [Abstract](https://arxiv.org/abs/2603.25251)
- [PDF](https://arxiv.org/pdf/2603.25251)

