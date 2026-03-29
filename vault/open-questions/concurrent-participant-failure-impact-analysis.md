---
created_at: '2026-03-29T18:59:43Z'
source_papers:
- '[[openalex-2603.25289-revealing-the-influence-of-participant-failures-on-model-qua]]'
title: Concurrent failure impact analysis
---

**Background:** Participant failures in cross-silo Federated Learning systems introduce complexity due to the high impact of losing unique local data contributions. In this study, only single participant crashes were analyzed.

**Question / Future Work:** Future work should analyze the impact of concurrent failures, such as multiple participants crashing simultaneously due to shared environmental factors like widespread network failures, and quantify how the aggregate data loss scales the negative impact on model quality.

**Why It Matters:** Understanding concurrent failures is necessary for designing robust fault-tolerance mechanisms that account for correlated failure modes common in large-world distributed systems.

**Evidence:** Despite that, in a real-world setting, it is possible that multiple participants can crash at the same time due to network failures. We assume that for all dataset types the impact will only increase as more missing participants result in more missing data in the process.