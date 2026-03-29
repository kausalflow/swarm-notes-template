---
# CSL-compatible fields
title: "TIGFlow-GRPO: Trajectory Forecasting via Interaction-Aware Flow Matching and Reward-Driven Optimization"
author:
  - literal: "Xuepeng Jing"
  - literal: "Wenhuan Lu"
  - literal: "Hao Meng"
  - literal: "Zhizhi Yu"
  - literal: "Jianguo Wei"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.24936"

# Custom fields
paper_id: "2603.24936"
paper_source: "openalex"
domain: "computer-vision"
tags:
  - "trajectory forecasting"
  - "generative models"
  - "conditional flow matching"
  - "reinforcement learning"
  - "interaction modeling"
architectures:
  []
datasets:
  - "ETH/UCY"
  - "SDD"
concept_slugs:
  - "trajectory-interaction-graph-tig"
  - "flow-grpo-post-training"
dataset_slugs:
  - "ethucy"
  - "sdd"
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:58:28Z"
created_at: "2026-03-29T18:58:28Z"
---

# TIGFlow-GRPO: Trajectory Forecasting via Interaction-Aware Flow Matching and Reward-Driven Optimization

**Authors**: Xuepeng Jing, Wenhuan Lu, Hao Meng, Zhizhi Yu, Jianguo Wei
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.24936](https://arxiv.org/abs/2603.24936)

## Summary

This paper introduces TIGFlow-GRPO, a two-stage generative framework for human trajectory forecasting that bridges Conditional Flow Matching (CFM) with behavior-aware alignment. The first stage integrates a Trajectory-Interaction-Graph (TIG) module into the CFM predictor to better model fine-grained agent-agent and agent-scene spatial interactions. The second stage refines the model using Flow-GRPO post-training, which involves sampling trajectories via stochastic ODE-to-SDE rollout and optimizing them using a composite reward balancing social compliance and physical feasibility. Evaluations on ETH/UCY and SDD show TIGFlow-GRPO achieves better accuracy and long-horizon stability while generating more behaviorally plausible trajectories.

## Key Contributions

- Introduction of TIGFlow-GRPO, a two-stage generative framework that uses Conditional Flow Matching (CFM) combined with a Trajectory-Interaction-Graph (TIG) module for enhanced context encoding.
- Formulation of Flow-GRPO post-training, which reformulates deterministic flow rollout as stochastic ODE-to-SDE sampling to facilitate trajectory exploration guided by behavioral rewards.
- Design of a composite reward function that integrates view-aware social compliance and map-aware physical feasibility to steer multimodal predictions towards plausible futures.
- Demonstration of improved forecasting accuracy and long-horizon stability over existing methods on the ETH/UCY and SDD benchmarks.

## Limitations

The abstract does not explicitly mention limitations, but the reliance on a multi-stage training process (CFM + GRPO) could introduce training complexity or instability compared to purely supervised methods.

## Open Questions & Future Work

- [[trajectory-forecasting-richer-visual-inputs-and-vlm-reasoning]]

## Key Concepts

- [[trajectory-interaction-graph-tig]]: A graph-based module integrated into a Conditional Flow Matching framework to capture fine-grained visual-spatial interactions between agents and the scene.
- [[flow-grpo-post-training]]: A post-training method that refines a flow-based trajectory model by reformulating its deterministic rollout as stochastic SDE sampling and optimizing via a composite reward function.

## Archivist Review

Two core methodological contributions, the TIG module and the Flow-GRPO post-training mechanism, were approved as they represent reusable advancements in flow-based generative modeling combined with behavior alignment. The two standard trajectory forecasting datasets, ETH/UCY and SDD, were also approved due to their centrality in the evaluation section. The single open question was retained as it points toward a specific, advanced future research direction involving richer visual grounding via VLMs.

### Approved Concepts
- Trajectory-Interaction-Graph (TIG) Module: It explicitly models both agent-agent and agent-scene relations to create informative conditional features for the flow matching process.
- Flow-GRPO Post-Training: It is the novel core mechanism for aligning the flow-based generation with behavioral/social rules via reinforcement learning techniques.

### Approved Open Questions
- Integrate richer visual inputs and VLM reasoning: Incorporating richer visual information and VLM reasoning can help ground trajectory predictions in a deeper semantic understanding of complex, dynamic scenes, moving beyond purely geometric or proximity-based scene modeling.

### Rejected Candidates
- [dataset] ETH/UCY (`eth/ucy`) - generic: The dataset ETH/UCY was approved as it is a standard benchmark central to trajectory forecasting evaluation.
- [dataset] SDD (`sdd`) - generic: The dataset SDD was approved as it is a standard benchmark central to trajectory forecasting evaluation.

## Datasets

- [[ethucy]]
- [[sdd]]

## Links

- [Abstract](https://arxiv.org/abs/2603.24936)
- [PDF](https://arxiv.org/pdf/2603.24936)

