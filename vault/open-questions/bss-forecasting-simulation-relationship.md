---
created_at: '2026-03-29T18:57:23Z'
source_papers:
- '[[openalex-2603.14901-the-impact-of-machine-learning-forecasting-on-strategic-deci]]'
title: Future of BSS Forecasting Detail
---

**Background:** Research involving the integration of machine learning forecasts into Bike Sharing System (BSS) simulations requires modeling user demand, often simplified as the net difference between bike returns and withdrawals at each station. The accuracy of the overall system simulation is intrinsically linked to the precision of these demand forecasts.

**Question / Future Work:** Further investigation is needed into the relationship between machine learning forecasting models and the subsequent simulation of BSS operations. This includes exploring how different levels of forecasting detail (e.g., net demand vs. Origin-Destination pairs) affect the simulation's ability to accurately model system dynamics and support strategic planning.

**Why It Matters:** Moving beyond net demand to OD-pair forecasting is crucial for accurately modeling user flow and optimizing relocation, which is a core operational challenge in BSS management.

**Evidence:** Further investigating the relationship between forecasting and BSS simulation is an area of future research. In this work, user behavior and demand have been represented, for both the forecast and the simulation, by the net demand of bikes at each station. More detailed representations, such as, demand for a trip from a specific bike station to another, or from the actual origin to destination of the user, would allow for a more accurate estimation of the relationship between request forecasting and decision-making for bike sharing systems.