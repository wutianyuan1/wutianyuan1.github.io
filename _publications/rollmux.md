---
title: "Weave: Efficient Co-Scheduling for Disaggregated RL Post-Training"
collection: publications
category: conf
permalink: /publication/rollmux
badge: 'OSDI 26'
excerpt: '<u>Tianyuan Wu</u>, Lunxi Cao, Yining Wei, Wei Gao, Yuheng Zhao, Dakai An, Shaopan Xiong, Zhiqiang Lv, Ju Huang, Siran Yang, Yinghao Yu, Jiamang Wang, Lin Qu, Wei Wang.'
date: 2025-12-12
venue: 'USENIX Symposium on Operating Systems Design and Implementation (OSDI), Seattle, July 2026.'
paperurl: 'https://arxiv.org/abs/2512.11306v1'
---

Rollout-training disaggregation is emerging as the standard architecture for Reinforcement Learning (RL) post-training, where memory-bound rollout and compute-bound training are physically disaggregated onto purpose-built clusters to maximize hardware efficiency. However, the strict synchronization required by on-policy algorithms introduces severe dependency bubbles, forcing one cluster to idle while the dependent phase is running on the other. We present Weave, a cluster scheduling framework that reclaims these bubbles through cross-cluster orchestration. Weave is built on the insight that the structural idleness of one job can be effectively utilized by the active phase of another. To realize this, we introduce the co-execution group abstraction, which partitions the cluster into isolated locality domains. This abstraction enables a two-tier scheduling architecture: an inter-group scheduler that optimizes job placement using conservative stochastic planning, and an intra-group scheduler that orchestrates a provably optimal round-robin schedule. The group abstraction also imposes a residency constraint, ensuring that massive model states remain cached in host memory to enable "warm-start" context switching. We evaluate Weave on a production-scale testbed with 328 H20 and 328 H800 GPUs. Weave improves cost efficiency by 1.84x over standard disaggregation and 1.38x over state-of-the-art co-located baselines, all while achieving 100% SLO attainment.
