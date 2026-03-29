---
created_at: '2026-03-29T18:58:51Z'
source_papers:
- '[[openalex-2603.25687-on-neural-scaling-laws-for-weather-emulation-through-continu]]'
title: Limits of Neural Scaling Extrapolation
---

**Background:** In scientific machine learning for weather forecasting, the relationship between model size, data size, and computational budget determines the optimal training configuration.

**Question / Future Work:** Investigating whether scaling laws hold when extending to significantly larger compute budgets (e.g., beyond $2.25 \\times 10^{21}$ FLOPs) and at higher spatial resolutions or with different data sampling strategies, to determine if the observed saturation in performance is a fundamental limit or an artifact of the current experimental setup (like multi-epoch training on the fixed ERA5 dataset).

**Why It Matters:** Understanding the long-term validity of scaling laws is crucial for planning resource allocation for future frontier-scale scientific models.

**Evidence:** Our results indicate that extrapolating to very large compute budgets with models exceeding a billion parameters shows signs of saturation. This may be due to the limited dataset size and the need to train for multiple epochs to reach these compute budgets.