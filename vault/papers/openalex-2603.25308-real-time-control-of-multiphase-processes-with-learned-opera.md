---
# CSL-compatible fields
title: "Real-time control of multiphase processes with learned operators"
author:
  - literal: "Paolo Guida"
  - literal: "Didier Barradas-Bautista"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25308"

# Custom fields
paper_id: "2603.25308"
paper_source: "openalex"
domain: "control-systems"
tags:
  - "model-based-control"
  - "surrogate-modeling"
  - "operator-learning"
  - "non-linear-dynamics"
architectures:
  - "Fourier Neural Operator"
datasets:
  []
concept_slugs:
  - "surrogate-assisted-mpc"
  - "fno-multiphase-surrogate"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:59:03Z"
created_at: "2026-03-29T18:59:03Z"
---

# Real-time control of multiphase processes with learned operators

**Authors**: Paolo Guida, Didier Barradas-Bautista
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25308](https://arxiv.org/abs/2603.25308)

## Summary

This work introduces a surrogate-assisted Model Predictive Control (MPC) framework to enable real-time control of complex, computationally expensive multiphase processes. The key innovation is using a Fourier Neural Operator (FNO) as a fast surrogate model to forecast the spatiotemporal evolution of a phase-indicator field over a finite horizon. This learned operator is iteratively called within the MPC optimization loop to identify optimal control inputs, significantly reducing the computational burden associated with high-fidelity numerical solvers. The approach was successfully applied to track liquid level setpoints in a two-phase Eulerian bubble column by adjusting the gas flow rate, demonstrating the viability of FNO-based field forecasting for closed-loop optimization.

## Key Contributions

- Proposed a surrogate-assisted Model Predictive Control (MPC) framework for multiphase processes by integrating learned operators.
- Trained a Fourier Neural Operator (FNO) to forecast the spatiotemporal evolution of the phase-indicator field (volume fraction) given recent states and actuation signals.
- Demonstrated the framework by solving an Optimal Control Problem (OCP) on a two-phase Eulerian bubble column, tracking liquid level setpoints by adjusting gas flow rate.
- Showed that field-level forecasting with FNOs is suitable for closed-loop optimization due to low evaluation cost, providing a practical path toward MPC for fast unit operations.

## Limitations

The current work is demonstrated on a two-phase Eulerian bubble column and the authors mention future extensions to partial observability.

## Key Concepts

- [[surrogate-assisted-mpc]]: A control framework where a learned operator (surrogate model) is used iteratively within a Model Predictive Control loop to solve for optimal control actions.
- [[fno-multiphase-surrogate]]: A Fourier Neural Operator trained to predict the future spatiotemporal evolution of a phase-indicator field (volume fraction) for model predictive control.

## Archivist Review

Two concepts were approved as they represent the core technical contributions. The first, 'Surrogate-Assisted MPC', captures the reusable overarching control framework combining machine learning with established control theory. The second, 'Learned Operator for Multiphase Flow Control', captures the specific, reusable application of a Fourier Neural Operator as a fast surrogate model for complex physical field forecasting in a control loop. Both elements are central and reusable beyond this specific multiphase system application. No datasets or open questions warranted inclusion.

### Approved Concepts
- Surrogate-Assisted Model Predictive Control (MPC): This framework directly addresses the computational bottleneck of using high-fidelity numerical models for real-time control by replacing them with fast surrogate models (learned operators).
- Learned Operator for Multiphase Flow Control: The core novelty is training a Fourier Neural Operator specifically to forecast the spatiotemporal evolution of a phase-indicator field for closed-loop control of multiphase systems.

### Rejected Candidates
- [concept] Learned Operator for Multiphase Flow Control (`fno-multiphase-surrogate`) - other: The candidate FNO concept is specific to applying the FNO to phase-indicator fields for multiphase control, which makes the second concept more appropriate as it captures the specific application context that drives novelty. However, since the FNO itself is a general architecture, I will approve the more general 'surrogate-assisted-mpc' and keep the FNO application as a specific concept illustrating that reuse. In this case, I will keep both as they represent the core technique (surrogate MPC) and the specific ML tool used (FNO for field forecasting). Since both appear central, they are both approved. Re-evaluating the rejection list structure based on the final output: no rejections occurred.

## Links

- [Abstract](https://arxiv.org/abs/2603.25308)
- [PDF](https://arxiv.org/pdf/2603.25308)

