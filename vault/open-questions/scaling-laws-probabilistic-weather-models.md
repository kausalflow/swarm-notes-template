---
created_at: '2026-03-29T18:58:51Z'
source_papers:
- '[[openalex-2603.25687-on-neural-scaling-laws-for-weather-emulation-through-continu]]'
title: Scaling Laws for Probabilistic Weather Models
---

**Background:** Weather dynamics are inherently chaotic, making probabilistic forecasts using metrics like CRPS more informative than deterministic forecasts using only MSE or RMSE.

**Question / Future Work:** Exploring the neural scaling behavior when training weather emulators using probabilistic objectives, such as diffusion objectives or CRPS-based ensemble training, and comparing these scaling trends against the deterministic scaling laws identified in this work.

**Why It Matters:** Establishing scaling laws for probabilistic models is necessary for applying resource allocation guidance to models designed for uncertainty quantification in chaotic systems.

**Evidence:** The main limitation of this paper is its focus on deterministic training of the weather model. . . Addressing this would involve training (or cooling down) models using diffusion objectives or CRPS-based ensemble training, and this may exhibit different scaling behaviors—this is left for future work.