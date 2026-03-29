---
# CSL-compatible fields
title: "A Distribution-to-Distribution Neural Probabilistic Forecasting Framework for Dynamical Systems"
author:
  - literal: "Tianlin Yang"
  - literal: "Hailiang Du"
  - literal: "Louis J. M. Aslett"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25370"

# Custom fields
paper_id: "2603.25370"
paper_source: "openalex"
domain: "time-series"
tags:
  - "probabilistic forecasting"
  - "uncertainty quantification"
  - "dynamical systems"
architectures:
  []
datasets:
  []
concept_slugs:
  - "distribution-to-distribution-d2d-forecasting"
  - "kernel-mean-embeddings-for-distribution-encoding"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:17Z"
created_at: "2026-03-29T18:57:17Z"
---

# A Distribution-to-Distribution Neural Probabilistic Forecasting Framework for Dynamical Systems

**Authors**: Tianlin Yang, Hailiang Du, Louis J. M. Aslett
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25370](https://arxiv.org/abs/2603.25370)

## Summary

This paper introduces a novel Distribution-to-Distribution (D2D) neural probabilistic forecasting framework designed to directly model the evolution of probability distributions in dynamical systems, addressing the limitation of trajectory-oriented methods. The architecture embeds input distributions using kernel mean embeddings, processes them through a replaceable neural forecasting module, and parameterizes the output predictive distribution via mixture density networks, enabling end-to-end learning. Demonstrated on the Lorenz63 chaotic system, the D2D model effectively captures complex distributional evolution and produces skillful probabilistic forecasts without relying on ensemble simulations. This work posits a new paradigm where predictive uncertainty is learned and propagated directly as a continuous object rather than indirectly inferred from sampled trajectories.

## Key Contributions

- Introduction of a Distribution-to-Distribution (D2D) neural forecasting framework that operates directly on predictive distributions rather than trajectories.
- The framework utilizes distributional encoding via kernel mean embeddings and distributional parameterization via mixture density networks within a single end-to-end architecture.
- Demonstrated the capability to capture nontrivial distributional evolution in the chaotic Lorenz63 dynamical system without explicit ensemble simulation.
- Achieved skillful probabilistic forecasts competitive with, and sometimes superior to, a simplified perfect model benchmark.

## Limitations

The current demonstration is restricted to the Lorenz63 chaotic dynamical system, and the generalization to more complex, high-dimensional, or real-world systems remains to be fully explored.

## Open Questions & Future Work

- [[joint-distribution-forecasting-challenge]]

## Key Concepts

- [[distribution-to-distribution-d2d-forecasting]]: A neural framework that learns to map an input predictive probability distribution to an output predictive probability distribution directly, bypassing trajectory-based simulation.
- [[kernel-mean-embeddings-for-distribution-encoding]]: Using kernel mean embeddings as a method to map arbitrary input probability distributions into a vector representation for consumption by a neural network.

## Archivist Review

Approved the central Distribution-to-Distribution (D2D) framework concept and the specific distributional encoding technique (Kernel Mean Embeddings) as they represent novel, reusable architectural components for probabilistic forecasting. One substantial open question regarding the scalability of joint distribution modeling was approved as it highlights a key limitation in extending this class of models. The Lorenz63 system was rejected as it is a specific, canonical test case rather than a general reusable dataset.

### Approved Concepts
- Distribution-to-Distribution (D2D) Neural Probabilistic Forecasting Framework: This is the core novel architectural framework proposed by the paper, designed to learn and propagate predictive distributions directly rather than through ensembles.
- Kernel Mean Embeddings for Distributional Encoding: This specific technique is used as the mechanism to encode a full probability distribution into a fixed-length representation suitable for the neural module.

### Approved Open Questions
- Scalable joint distribution parameterization: The ability to model the full joint predictive distribution is crucial for accurately capturing cross-variable dependencies and propagating correlated uncertainty in multi-dimensional dynamical systems.

### Rejected Candidates
- [dataset] Lorenz63 (`lorenz63`) - paper_local: The Lorenz63 system is a well-known benchmark for chaotic systems and is not a general-purpose dataset warranting a permanent vault entry.

## Links

- [Abstract](https://arxiv.org/abs/2603.25370)
- [PDF](https://arxiv.org/pdf/2603.25370)

