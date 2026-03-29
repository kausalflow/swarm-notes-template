---
created_at: '2026-03-29T18:58:51Z'
source_papers:
- '[[openalex-2603.25687-on-neural-scaling-laws-for-weather-emulation-through-continu]]'
title: Scaling Internal Transformer Resolution
---

**Background:** The transformer resolution (sequence length) is determined by the spatial grid size and the patch size used for input embedding.

**Question / Future Work:** Investigating the scaling behavior as a function of internal Transformer resolution, which can be treated as an additional independent scaling dimension by systematically varying the input patch size while keeping the overall spatial grid size fixed for the scaling tests.

**Why It Matters:** Understanding how sequence length scaling interacts with model size and data scaling provides a more complete picture of the full scaling landscape for spatiotemporal models.

**Evidence:** Our patch size is fixed for the scaling tests, but the internal Transformer resolution (sequence length) represents another dimension for systematic scaling studies.