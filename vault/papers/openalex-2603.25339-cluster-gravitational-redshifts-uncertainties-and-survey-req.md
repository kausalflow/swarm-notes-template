---
# CSL-compatible fields
title: "Cluster gravitational redshifts: uncertainties and survey requirements"
author:
  - literal: "Eleni Tsaprazi"
  - literal: "Giorgio F. Lesci"
  - literal: "Federico Marulli"
  - literal: "Alan F. Heavens"
  - literal: "Enrico Maraboli"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25339"

# Custom fields
paper_id: "2603.25339"
paper_source: "openalex"
domain: "cosmology"
tags:
  - "cosmology"
  - "modified gravity"
  - "galaxy clusters"
  - "spectroscopic survey"
  - "forecasting"
architectures:
  []
datasets:
  []
concept_slugs:
  - "cluster-gravitational-redshifts-mg-probe"
  - "five-parameter-hod-model"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T19:00:17Z"
created_at: "2026-03-29T19:00:17Z"
---

# Cluster gravitational redshifts: uncertainties and survey requirements

**Authors**: Eleni Tsaprazi, Giorgio F. Lesci, Federico Marulli, Alan F. Heavens, Enrico Maraboli
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25339](https://arxiv.org/abs/2603.25339)

## Summary

This paper develops an end-to-end forecasting pipeline to quantify the uncertainties affecting cluster gravitational redshifts as a probe of modified gravity, parameterized by the linear rescaling $\alpha_\mathrm{MG}$. The pipeline simulates galaxy catalogues using a five-parameter Halo Occupation Distribution (HOD) and incorporates various observational uncertainties. The authors find that the intracluster velocity dispersion establishes a hard limit on redshift precision improvement ($σ_z\sim 10^{-4}(1+z)$) and that accurate cluster centering is crucial, as mis-centring introduces systematic biases mimicking new physics. Consequently, the study concludes that shallow, narrow spectroscopic surveys are preferable to deep, wide photometric surveys for obtaining tight constraints on modified gravity models.

## Key Contributions

- Developed an end-to-end forecasting pipeline to assess the precision of cluster gravitational redshifts ($α_\mathrm{MG}$) as a probe for modified gravity.
- Determined that intracluster velocity dispersion sets an effective floor for redshift precision, with no benefit gained beyond $σ_z\sim 10^{-4}(1+z)$.
- Found that shallow, narrower spectroscopic surveys are superior to deep, wide photometric surveys for achieving precise modified gravity constraints using this method.
- Identified that accurate determination of cluster centers is essential, as mis-centring can mimic significant departures from General Relativity.

## Limitations

The analysis does not find appreciable biases from baryonic deviations (NFW profile) or velocity anisotropies, but future work may require deeper investigation into these non-GR effects.

## Open Questions & Future Work

- [[accurate-cluster-center-determination-for-modified-gravity-tests]]
- [[self-consistent-modified-gravity-simulations-for-haloes]]
- [[exploring-advanced-modified-gravity-parameterizations]]

## Key Concepts

- [[cluster-gravitational-redshifts-mg-probe]]: Using the gravitational redshift of galaxies within galaxy clusters to test deviations from General Relativity (GR) parameterized by $α_\\mathrm{MG}$.
- [[five-parameter-hod-model]]: A statistical framework used to model the number and spatial distribution of observable galaxies residing within dark matter halos based on halo mass.

## Archivist Review

Approved two central concepts, primarily the overarching cosmological probe being investigated and the specific HOD modeling technique used within the simulation. Three substantial open questions were approved focusing on critical unresolved technical issues: accurate centering, the necessity of self-consistent modified-gravity simulations, and the limitations of the current parameterization scheme. No datasets were approved as the paper discusses future surveys rather than using established benchmark datasets.

### Approved Concepts
- Cluster Gravitational Redshifts as a Probe of Modified Gravity: The entire paper is focused on quantifying the precision of this specific cosmological probe ($α_\\mathrm{MG}$) under various observational conditions.
- Halo Occupation Distribution (HOD) Modeling for Cluster Membership: The HOD model is a critical, specific component of the end-to-end simulation pipeline used to assign galaxies to simulated dark matter halos.

### Approved Open Questions
- Accurate cluster center determination: Accurate cluster center determination is paramount because mis-centring can mimic significant departures from General Relativity (GR), potentially leading to false detections of new physics, which invalidates the scientific goal of the measurement.
- Self-consistent modified gravity simulations: Current analysis uses GR-based halo catalogues, which means the structural properties of halos themselves (which influence the gravitational redshift signal) are not being tested under the modified gravity scenarios being investigated, limiting the model's predictive power in a full modified gravity universe.
- Advanced modified gravity parameterizations: Using a more complex or physically motivated parameterization could allow for tighter or more physically meaningful constraints on specific modified gravity theories, which is the ultimate goal of the gravitational redshift probe.

### Rejected Candidates
- [concept] End-to-End Forecasting Pipeline for Gravitational Redshifts (`end-to-end-forecasting-pipeline`) - paper_local: The pipeline is a specific implementation for this problem, not a generally reusable, named methodological component.
- [concept] $\\alpha_\\mathrm{MG}$ Parameterization (`alpha-mg-parameter`) - subcomponent_of_broader_mechanism: This is a generic, localized parameter used to parameterize modifications to GR within this specific framework, which is better captured by the broader concept.
- [concept] Intracluster Velocity Dispersion Floor (`intracluster-velocity-dispersion-floor`) - low_impact: This is a specific finding/limitation derived from the physical model, not a general reusable methodology or concept.
- [concept] Preference for Shallow, Narrow Spectroscopic Surveys (`spectroscopic-surveys-vs-photometric-surveys-preference`) - paper_local: This is a conclusion based on the specific forecasting pipeline, not a general methodological concept that would recur.
- [concept] Cluster Mis-Centring as a Systematic Bias (`cluster-miscentring-systematic`) - paper_local: This is a specific systematic effect identified within the simulation, not a general reusable concept or method.
- [dataset] Spectroscopic Stage-5 Experiment and Widefield Spectroscopic Telescope (`spectroscopic-stage-5-experiment-and-widetelescope`) - low_impact: These are names of future observational surveys, not established benchmark datasets used for evaluating current methods.

## Links

- [Abstract](https://arxiv.org/abs/2603.25339)
- [PDF](https://arxiv.org/pdf/2603.25339)

