---
# CSL-compatible fields
title: "The impact of machine learning forecasting on strategic decision-making for bike sharing systems"
author:
  - literal: "Enrico Angelelli"
  - literal: "Andrea Mor"
  - literal: "Carlotta Orsenigo"
  - literal: "M. Grazia Speranza"
  - literal: "Carlo Vercellis"
issued:
  date-parts:
    - [2026, 3, 27]
url: "https://arxiv.org/abs/2603.14901"

# Custom fields
paper_id: "2603.14901"
paper_source: "openalex"
domain: "time-series"
tags:
  - "forecasting"
  - "simulation"
  - "decision-making"
  - "optimization"
architectures:
  []
datasets:
  - "Brescia bike sharing system data"
concept_slugs:
  - "bike-sharing-flow-forecasting"
  - "simulation-aided-decision-support-for-logistics"
dataset_slugs:
  - "brescia-bike-sharing-system-data"
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T18:57:23Z"
created_at: "2026-03-29T18:57:23Z"
---

# The impact of machine learning forecasting on strategic decision-making for bike sharing systems

**Authors**: Enrico Angelelli, Andrea Mor, Carlotta Orsenigo, M. Grazia Speranza, Carlo Vercellis
**Date**: 2026-03-27
**Paper ID**: [openalex:2603.14901](https://arxiv.org/abs/2603.14901)

## Summary

This paper explores the use of machine learning models to forecast the critical metric of net flow (returns minus withdrawals) at each station in a bike-sharing system. These forecasts are then embedded within a simulation framework used for modeling daily operational dynamics, such as bike relocation, and supporting long-term strategic decisions. The authors evaluate the quality of the ML predictions by comparing them against alternative methods and, crucially, by quantifying how the improved forecast accuracy affects the overall performance and output quality of the integrated simulation model. The evaluation is grounded using real-world data collected from the bike-sharing system operating in Brescia, Italy.

## Key Contributions

- Application of machine learning techniques to forecast the net difference between bike returns and withdrawals at individual stations in a bike-sharing system.
- Integration of these ML-based forecasts into a simulation framework designed to model daily dynamics and support long-term decision-making, including bike relocation strategies.
- Evaluation framework that assesses forecast quality by comparing ML models against alternatives and by analyzing the impact of the forecasts on the overall performance of the simulation output.

## Limitations

The evaluation is based on a single real-world system (Brescia), which might limit the generalizability of the observed impacts.

## Open Questions & Future Work

- [[bss-forecasting-simulation-relationship]]

## Key Concepts

- [[bike-sharing-flow-forecasting]]: Forecasting the net difference between bike returns and withdrawals at specific stations within a bike-sharing system.
- [[simulation-aided-decision-support-for-logistics]]: Using machine learning forecasts within a simulation environment to model daily dynamics and support strategic decisions, such as bike relocation, in a bike-sharing system.

## Archivist Review

Two concepts were approved as they capture the specific problem domain (forecasting net flow) and the novel application paradigm (integrating forecasts into operational simulation for decision support). One dataset, the Brescia system data, was approved as it is the specific named data source used for evaluation. One open question was approved as it points to a specific, unresolved gap in modeling detail (net demand vs. Origin-Destination pairs) within this application domain.

### Approved Concepts
- Bike Sharing Flow Forecasting: This is the specific forecasting task that the paper applies ML techniques to, focusing on net flow rather than just demand.
- Simulation-Aided Decision Support for Bike Sharing: The core novelty lies in *integrating* ML forecasts with a simulation framework to directly influence strategic/operational decisions (like bike relocation).

### Approved Open Questions
- Future of BSS Forecasting Detail: Moving beyond net demand to OD-pair forecasting is crucial for accurately modeling user flow and optimizing relocation, which is a core operational challenge in BSS management.

### Rejected Candidates
- [dataset] Brescia bike sharing system data (`Brescia bike sharing system data`) - generic: The dataset is a named, real-world dataset central to the evaluation, but given the scarcity rule, it is approved as the only dataset candidate.

## Datasets

- [[brescia-bike-sharing-system-data]]

## Links

- [Abstract](https://arxiv.org/abs/2603.14901)
- [PDF](https://arxiv.org/pdf/2603.14901)

