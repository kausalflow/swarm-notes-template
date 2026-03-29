---
created_at: '2026-03-29T19:00:01Z'
source_papers:
- '[[openalex-2603.25446-implementation-of-a-near-realtime-recording-and-reporting-sy]]'
title: Expand ML Detector to Other Burst Types
---

**Background:** The capability to detect and analyze solar radio bursts is crucial for space weather monitoring and forecasting, but existing systems often have high latency or insufficient sensitivity.

**Question / Future Work:** The detector was trained exclusively on synthetic type III and type IIIb radio bursts, making it currently optimized only for electron-beam related activity. Future work should involve expanding the training set to include other critical burst types, specifically type II bursts, which are key signatures of CME-driven shocks, as well as other burst classes and representative noise-storm/background scenarios.

**Why It Matters:** Type II bursts are vital as they trace CME-driven shocks, which are primary accelerators of large Solar Energetic Particle (SEP) events, making their inclusion critical for comprehensive space weather early warning systems.

**Evidence:** Future work will expand the detector beyond the current type III/type IIIb training set. In particular, type II bursts—key signatures of CME-driven shocks—and other burst classes (e.g., type V) are not yet represented in the training data, so the present system should be viewed as optimized for type III-related electron-beam activity. We are building a larger multi-type labeled dataset (including type II, additional burst classes, and noise-storm/background scenarios).