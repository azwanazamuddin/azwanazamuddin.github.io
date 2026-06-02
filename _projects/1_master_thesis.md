---
layout: page
title: Master's Thesis
description: A Scalable Computational Framework for Activity-Based Dynamic Discrete Choice Models
importance: 1
category: research
---

**Supervisor:** Prof. Makoto Chikaraishi, Hiroshima University

Activity-based dynamic discrete choice models (DDCM) are among the most behaviorally realistic tools for travel demand analysis, but exact estimation at city scale has been computationally out of reach — the theoretical state space for a realistic model runs to hundreds of millions of states, requiring thousands of CPU-hours.

This thesis develops a scalable computational framework built around three contributions:

- **Reachability-based state space reduction** — a BFS-based pruning algorithm that retains only states reachable from the observed population, reducing the state space from ~146M to ~1.5M (99% reduction) while preserving exact computation
- **Sparse graph representation** — using compressed sparse row (CSR) format to bring memory requirements from ~6.7 TB to ~6.5 GB
- **GPU-accelerated backward induction** — reducing wall time from ~69 hours to ~105 seconds on the Higashi-Hiroshima travel diary dataset (825 persons, 10-parameter model)

The result is the first demonstration of exact, welfare-consistent city-scale DDCM estimation on real data, producing a fully converged likelihood at ll = −28,708.6.

This work directly motivates the longer-term research agenda on [Structural-IRL](/projects/2_structural_irl), which extends these foundations to welfare-preserving tractability at full city scale.

**Conference papers from this work:**
- *Scalable and Exact Activity-Based Dynamic Discrete Choice Models via Reachability and Sparse Graph Computation* — APTE 2026 (accepted, oral presentation, July 2026)
- *A Reachability-Based Computational Framework for Population-Scale Activity-Based Dynamic Discrete Choice Models* — ICMC 2026 (accepted, oral presentation, July 2026)
