---
created_at: '2026-03-29T18:59:54Z'
source_papers:
- '[[openalex-2603.25251-does-explanation-correctness-matter-linking-computational-xa]]'
title: Finer-Grained Correctness Link
---

**Background:** The field of Explainable Artificial Intelligence (XAI) heavily relies on functional metrics, such as correctness, to assess the quality of explanations, assuming these metrics translate to improved human understanding.

**Question / Future Work:** The specific relationship between human understanding (measured via forward simulation accuracy) and functional explanation correctness needs further testing, particularly in the narrow range between 85% and 100% correctness, which is where practical differences between XAI methods often occur.

**Why It Matters:** Resolving this gap is critical because if functional improvements in this high-correctness range do not yield corresponding human benefits, resources spent optimizing for these small functional gains may be misallocated.

**Evidence:** The unresolved comparison between 85% and 100% correctness highlights the need for finer granularity in the 70–100% range, which is where practical differences between XAI methods often fall.