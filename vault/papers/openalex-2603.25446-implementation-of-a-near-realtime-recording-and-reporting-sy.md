---
# CSL-compatible fields
title: "Implementation of a Near-Realtime Recording and Reporting System of Solar Radio Bursts"
author:
  - literal: "Peijin Zhang"
  - literal: "Anastasia Kuske"
  - literal: "Bin Chen"
  - literal: "Mengjia Xu"
  - literal: "Gelu M. Nita"
  - literal: "Marin M. Anderson"
  - literal: "Judd D. Bowman"
  - literal: "Ruby Byrne"
  - literal: "Morgan Catha"
  - literal: "Xingyao Chen"
  - literal: "Sherry Chhabra"
  - literal: "Larry D'Addario"
  - literal: "Ivey Davis"
  - literal: "Jayce Dowell"
  - literal: "Katherine Elder"
  - literal: "Dale Gary"
  - literal: "Gregg Hallinan"
  - literal: "Charlie Harnach"
  - literal: "Greg Hellbourg"
  - literal: "Jack Hickish"
  - literal: "Rick Hobbs"
  - literal: "David Hodge"
  - literal: "Mark Hodges"
  - literal: "Yuping Huang"
  - literal: "Andrea Isella"
  - literal: "Daniel C. Jacobs"
  - literal: "Ghislain Kemby"
  - literal: "John T. Klinefelter"
  - literal: "Matthew Kolopanis"
  - literal: "Nikita Kosogorov"
  - literal: "James Lamb"
  - literal: "Casey Law"
  - literal: "Nivedita Mahesh"
  - literal: "Surajit Mondal"
  - literal: "Brian O'Donnell"
  - literal: "Kathryn Plant"
  - literal: "Corey Posner"
  - literal: "Travis Powell"
  - literal: "Vinand Prayag"
  - literal: "Andres Rizo"
  - literal: "Andrew Frederic Romero-Wolf"
  - literal: "Jun Shi"
  - literal: "Greg Taylor"
  - literal: "Jordan Trim"
  - literal: "Mike Virgin"
  - literal: "Akshatha Vydula"
  - literal: "Sandy Weinreb"
  - literal: "Scott White"
  - literal: "D. P. Woody"
  - literal: "Sijie Yu"
  - literal: "Thomas Zentmeyer"
issued:
  date-parts:
    - [2026, 3, 26]
url: "https://arxiv.org/abs/2603.25446"

# Custom fields
paper_id: "2603.25446"
paper_source: "openalex"
domain: "other"
tags:
  - "scientific machine learning"
  - "astrophysics"
  - "real-time systems"
  - "object detection"
architectures:
  - "YOLO"
datasets:
  []
concept_slugs:
  - "type-iii-radio-burst-identification"
  - "physics-based-synthetic-data-generation"
dataset_slugs:
  []
skill: "TimeSeriesSkill"
processed_at: "2026-03-29T19:00:01Z"
created_at: "2026-03-29T19:00:01Z"
---

# Implementation of a Near-Realtime Recording and Reporting System of Solar Radio Bursts

**Authors**: Peijin Zhang, Anastasia Kuske, Bin Chen, Mengjia Xu, Gelu M. Nita, Marin M. Anderson, Judd D. Bowman, Ruby Byrne, Morgan Catha, Xingyao Chen, Sherry Chhabra, Larry D'Addario, Ivey Davis, Jayce Dowell, Katherine Elder, Dale Gary, Gregg Hallinan, Charlie Harnach, Greg Hellbourg, Jack Hickish, Rick Hobbs, David Hodge, Mark Hodges, Yuping Huang, Andrea Isella, Daniel C. Jacobs, Ghislain Kemby, John T. Klinefelter, Matthew Kolopanis, Nikita Kosogorov, James Lamb, Casey Law, Nivedita Mahesh, Surajit Mondal, Brian O'Donnell, Kathryn Plant, Corey Posner, Travis Powell, Vinand Prayag, Andres Rizo, Andrew Frederic Romero-Wolf, Jun Shi, Greg Taylor, Jordan Trim, Mike Virgin, Akshatha Vydula, Sandy Weinreb, Scott White, D. P. Woody, Sijie Yu, Thomas Zentmeyer
**Date**: 2026-03-26
**Paper ID**: [openalex:2603.25446](https://arxiv.org/abs/2603.25446)

## Summary

This work presents the design and implementation of a near-realtime system at the Owens Valley Radio Observatory Long Wavelength Array for recording and reporting solar radio bursts, crucial for space weather monitoring. The system captures data directly from a realtime buffer, generating live dynamic spectrograms, and employs a deep-learning module based on the YOLO architecture to automatically identify Type III radio bursts. This identifier was trained using synthetic bursts generated from a physics-based model to ensure high accuracy and robustness in detection. The entire pipeline enables the continuous streaming of radio spectra and automatic reporting of detected Type III bursts within approximately 10 seconds of their actual occurrence.

## Key Contributions

- Development and implementation of a near-realtime recording and reporting system for solar radio bursts using the Owens Valley Radio Observatory Long Wavelength Array.
- Integration of a deep-learning-based Type III radio burst identification module, based on a YOLO architecture, directly into the live data stream.
- Achieving a low-latency reporting time of approximately 10 seconds from event occurrence to automated report generation for Type III bursts.
- Training the burst identifier using synthetic Type III radio bursts generated via a physics-based model for enhanced accuracy and robustness.

## Limitations

The system is currently specialized for Type III radio bursts, limiting its immediate application to other solar or space weather phenomena.

## Open Questions & Future Work

- [[solar-radio-burst-detector-multi-class-expansion]]

## Key Concepts

- [[type-iii-radio-burst-identification]]: A deep learning module specifically designed to identify transient Type III solar radio bursts within dynamic spectrograms.
- [[physics-based-synthetic-data-generation]]: The generation of synthetic training data for a deep learning model based on underlying physical simulation models of solar radio emissions.

## Archivist Review

Two concepts were approved, focusing on the specialized signal identification task (Type III bursts) and the novel training data augmentation strategy (physics-based synthetic data). The YOLO architecture was rejected as a generic component. One open question was approved as it specifies a crucial, unresolved expansion of the detection capability to include Type II bursts, which are vital for space weather forecasting. No datasets were approved as the paper focuses on system implementation rather than benchmarking a new time series dataset.

### Approved Concepts
- Type III Radio Burst Identification: This is the specific astrophysical phenomenon the system is designed to detect and report in near-realtime, crucial for space weather applications.
- Physics-Based Synthetic Data Generation for Bursts: Using physics-based models to create synthetic training data is a novel approach to overcome the scarcity or variability of real-world event data for training detectors.

### Approved Open Questions
- Expand ML Detector to Other Burst Types: Type II bursts are vital as they trace CME-driven shocks, which are primary accelerators of large Solar Energetic Particle (SEP) events, making their inclusion critical for comprehensive space weather early warning systems.

### Rejected Candidates
- [concept] YOLO architecture (`yolo`) - not_novel: The YOLO architecture is a generic, widely adopted object detection framework, not a novel contribution specific to this paper.
- [concept] Near-Realtime Radio Burst Reporting System (`near-realtime-radio-burst-reporting-system`) - paper_local: This is a system implementation description rather than a distinct, reusable algorithmic or methodological concept.
- [concept] Live Radio Dynamic Spectrogram Streaming (`live-radio-dynamic-spectrogram-streaming`) - generic: This refers to standard data processing and presentation techniques for radio astronomy data, not a novel ML concept.

## Links

- [Abstract](https://arxiv.org/abs/2603.25446)
- [PDF](https://arxiv.org/pdf/2603.25446)

