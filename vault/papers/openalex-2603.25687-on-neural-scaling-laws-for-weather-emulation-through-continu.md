---
# CSL-compatible fields
title: "On Neural Scaling Laws for Weather Emulation through Continual Training"
author:
  - literal: "Shashank Subramanian"
  - literal: "Alexander Kiefer"
  - literal: "Arnur Nigmetov"
  - literal: "Amir Gholami"
  - literal: "Dmitriy Morozov"
  - literal: "Michael W. Mahoney"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25687"

# Custom fields
paper_id: "2603.25687"
paper_source: "openalex"
domain: "time-series"
tags:
  - "neural scaling laws"
  - "weather forecasting"
  - "scientific machine learning"
  - "training methodology"
  - "optimization"
architectures:
  - "Swin Transformer"
datasets:
  []
concept_slugs:
  - "continual-training-with-cooldowns"
  - "iso-flop-curves-weather-emulation"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:51Z"
created_at: "2026-03-29T18:58:51Z"
---

# On Neural Scaling Laws for Weather Emulation through Continual Training

**Authors**: Shashank Subramanian, Alexander Kiefer, Arnur Nigmetov, Amir Gholami, Dmitriy Morozov, Michael W. Mahoney
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25687](https://arxiv.org/abs/2603.25687)

## Summary

This paper investigates neural scaling laws within Scientific Machine Learning, focusing on weather forecasting emulation using a minimalist Swin Transformer architecture. The authors propose using continual training with constant learning rates and periodic cooldowns as an efficient strategy, demonstrating it follows predictable scaling trends and surpasses standard learning schedules. They further analyze compute trade-offs by constructing IsoFLOP curves to identify compute-optimal training regimes for resource allocation. The cooldown phases were shown to improve performance, enabling more accurate, multi-step predictions over longer forecast horizons.

## Key Contributions

- Demonstrated that minimal Swin Transformer models trained with continual training (constant learning rates and periodic cooldowns) follow predictable neural scaling laws for weather emulation.
- Showed that the proposed continual training strategy outperforms standard cosine learning rate schedules.
- Established that cooldown phases can be leveraged to improve downstream performance, specifically enabling longer forecast horizons and sharper predictions via spectral loss adjustments.
- Constructed IsoFLOP curves across various compute budgets to identify compute-optimal training regimes for weather emulation tasks.

## Limitations

The study explores scaling in a "minimal, scalable, general-purpose Swin Transformer architecture," implying the findings might not generalize directly to all specialized weather models. Extrapolation highlights potential performance limits but does not fully resolve them.

## Open Questions & Future Work

- [[weather-scaling-law-extrapolation-limits]]
- [[scaling-laws-probabilistic-weather-models]]
- [[scaling-architecture-dependence-sciml]]
- [[scaling-transformer-internal-resolution]]

## Key Concepts

- [[continual-training-with-cooldowns]]: An efficient training strategy for neural networks involving constant learning rates punctuated by periodic cooldown phases, which can be repurposed to enhance downstream performance metrics like forecast horizon accuracy.
- [[iso-flop-curves-weather-emulation]]: Curves that map out the combinations of model size, dataset size, and computational budget that yield the same performance level, used here to identify compute-optimal training regimes in weather emulation.

## Archivist Review

Two concepts were approved: the specific training methodology 'Continual Training with Cooldowns' and the resource-optimization analysis technique 'IsoFLOP Curves for Weather Emulation', as both are central and reusable contributions to ML optimization. Four substantial open questions were approved, focusing on the limits of scaling extrapolation, scaling for probabilistic models, architectural dependence, and internal resolution scaling, as these represent critical avenues for future work in scientific ML scaling laws. Generic architectural choices and specific implementation tricks were rejected as non-reusable concepts.

### Approved Concepts
- Continual Training with Cooldowns: This specific training schedule (continual training with periodic cooldowns) is proposed as an efficient strategy that outperforms standard schedules and enables specific improvements like better multi-step rollouts.
- IsoFLOP Curves for Weather Emulation: IsoFLOP curves provide a formal method for identifying compute-optimal training regimes, which is a crucial concept for resource allocation in large-scale scientific modeling.

### Approved Open Questions
- Limits of Neural Scaling Extrapolation: Understanding the long-term validity of scaling laws is crucial for planning resource allocation for future frontier-scale scientific models.
- Scaling Laws for Probabilistic Weather Models: Establishing scaling laws for probabilistic models is necessary for applying resource allocation guidance to models designed for uncertainty quantification in chaotic systems.
- Scaling Behavior Across Architectures: It is unknown whether the identified compute-optimal regimes are universal across different architectural paradigms prevalent in Scientific Machine Learning.
- Scaling Internal Transformer Resolution: Understanding how sequence length scaling interacts with model size and data scaling provides a more complete picture of the full scaling landscape for spatiotemporal models.

### Rejected Candidates
- [concept] Swin Transformer (`swin-transformer`) - subcomponent_of_broader_mechanism: The use of a Swin Transformer is an implementation detail of the chosen architecture, not a novel, generalizable ML mechanism introduced by the paper.
- [concept] Spectral Loss Adjustments (`spectral-loss-adjustments`) - subcomponent_of_broader_mechanism: This is described as a means to achieve sharper predictions enabled by cooldowns, making it a specific application/detail rather than a reusable, core conceptual contribution.
- [concept] IsoFLOP Curves (`iso-flop-curves`) - duplicate_existing: The general concept of IsoFLOP curves is a well-established idea; the paper's contribution is the specific *application* of constructing them for weather emulation to find optimal regimes, which is captured by the more specific concept `iso-flop-curves-weather-emulation`.

## Links

- [Abstract](https://arxiv.org/abs/2603.25687)
- [PDF](https://arxiv.org/pdf/2603.25687)

