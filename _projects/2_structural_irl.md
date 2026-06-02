---
layout: page
title: Structural-IRL
description: Tractable welfare measurement in activity-based dynamic discrete choice models
importance: 2
category: research
---

**Long-term research agenda (JSPS DC1 application)**

A central question in transport policy is: does this policy make residents better or worse off, and by how much? Activity-based dynamic discrete choice models (DDCM) can answer this with behavioral realism — but exact welfare estimation has remained computationally intractable at city scale.

This research develops **Structural Inverse Reinforcement Learning (Structural-IRL)**, an algorithm that resolves this barrier by exploiting two proven mathematical connections:

1. DDCM estimation is structurally equivalent to **inverse reinforcement learning (IRL)**
2. DDCM backward induction shares the same computational graph as **graph neural networks (GNN)**

These connections allow deep learning and reinforcement learning methods to be incorporated into DDCM estimation — but only under conditions that preserve the welfare guarantee. Structural-IRL establishes those conditions and builds an algorithm that is both tractable and welfare-exact.

**Research themes:**
- **Theme 1** — Establish the conditions under which RL/DL connections preserve the welfare guarantee
- **Theme 2** — Design and implement Structural-IRL satisfying those conditions
- **Theme 3** — Empirical validation against the exact estimation baseline; city-scale spatial welfare analysis

**Policy motivation:**  
For a new bus rapid transit corridor, existing methods estimate aggregate ridership or average travel-time savings. Structural-IRL can estimate, for each household, the net change in daily well-being — identifying which neighborhoods gain, which lose, and where complementary measures are needed.

**Foundation:**  
Built on completed master's thesis work ([exact DDCM framework](/projects/1_master_thesis)) — 825 persons, Higashi-Hiroshima, exact estimation in ~17 hours on GPU.
