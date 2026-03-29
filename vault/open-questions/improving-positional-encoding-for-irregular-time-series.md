---
created_at: '2026-03-29T18:57:33Z'
source_papers:
- '[[openalex-2603.25597-spatiotemporal-system-forecasting-with-irregular-time-steps]]'
title: Advanced positional encoding for irregular time steps
---

**Background:** The model relies on sinusoidal positional embeddings to encode temporal ordering, which may not optimally capture relative temporal relationships in irregular time series compared to newer methods.

**Question / Future Work:** Exploring and implementing advanced positional embedding techniques, such as Attention with Linear Biases (ALiBi) or Rotary Position Embedding (RoPE), within the masked autoencoder framework to better represent relative temporal relationships across irregularly sampled time steps.

**Why It Matters:** The choice of positional encoding directly impacts how well the model understands the sequence timing, which is crucial for irregular time series forecasting accuracy.

**Evidence:** Future work could consider advanced positional embedding techniques, such as Attention with Linear Biases (ALiBi) [82] and Rotary Position Embedding (RoPE) [83], which can better capture relative temporal relationships without explicit positional encodings.