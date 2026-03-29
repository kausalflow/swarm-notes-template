---
created_at: '2026-03-29T18:59:43Z'
source_papers:
- '[[openalex-2603.25289-revealing-the-influence-of-participant-failures-on-model-qua]]'
title: Data-agnostic impact prediction
---

**Background:** In cross-silo Federated Learning (FL), participant contribution measures are often used to infer the importance of a participant to the overall model training process.

**Question / Future Work:** A suitable measurement for predicting the impact of a missing participant must be developed that is precise and does not require access to the server-side dataset (or any portion of participant data), as this requirement is often infeasible in real-world FL scenarios.

**Why It Matters:** Developing data-agnostic, low-overhead contribution metrics is crucial for real-time, practical fault detection and response in FL systems where data privacy prohibits centralized data access for validation.

**Evidence:** However, to calculate the SVs, a server-side dataset is required. In many real-world cases, sending a part of the participants data or using a public dataset is not feasible. Here, a suitable measurement is necessary that is precise and does not require server-side data.