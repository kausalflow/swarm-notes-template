---
created_at: '2026-03-29T18:58:51Z'
source_papers:
- '[[openalex-2603.25687-on-neural-scaling-laws-for-weather-emulation-through-continu]]'
title: Scaling Behavior Across Architectures
---

**Background:** Deep learning models for weather emulation can be structured using various architectures that incorporate domain knowledge, such as the geometric inductive biases used in Neural Operators or graph-based models.

**Question / Future Work:** Systematically studying neural scaling laws using different architectural backbones, such as those incorporating geometric inductive biases (e.g., Spherical Fourier Neural Operators or Graph Neural Networks), to determine if the observed scaling behavior is intrinsic to the task or dependent on the minimalist Transformer architecture chosen.

**Why It Matters:** It is unknown whether the identified compute-optimal regimes are universal across different architectural paradigms prevalent in Scientific Machine Learning.

**Evidence:** Another possible limitation is the focus on Transformer architectures. While this focus is intentional to demonstrate that simple architectures can scale and perform competitively, it remains important to explore other architecture types, such as FourCastNet [Bonev et al., 2025], which incorporates geometric inductive biases through spherical transforms within the neural operator framework, or graph-based approaches like GraphCast [Lam et al., 2023].