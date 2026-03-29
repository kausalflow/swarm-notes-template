---
created_at: '2026-03-29T18:57:44Z'
source_papers:
- '[[openalex-2603.25217-modeling-and-forecasting-tail-risk-spillovers-a-component-ba]]'
title: CAViaR Spillover Component Persistence
---

**Background:** Conditional Autoregressive Value at Risk (CAViaR) models capture the time-varying dynamics of conditional quantiles for asset returns.

**Question / Future Work:** Investigate the implications of the estimated autoregressive coefficient for the spillover component ($\\hat{\\varphi}_1$) being close to zero in the CAViaR-SE models, and how this impacts the interpretation of persistence versus absorption of dynamics by the spillover proxy.

**Why It Matters:** The finding that $\\hat{\\varphi}_1 \\approx 0$ suggests that the spillover component is driven almost entirely by the exogenous proxy rather than its own persistence, leading to a reallocation of persistence to the proper risk component, which warrants further theoretical and empirical investigation regarding the nature of the spillover dynamics.

**Evidence:** even though the estimated autoregressive coefficient $\\hat{\\varphi}_1$ is close to zero.