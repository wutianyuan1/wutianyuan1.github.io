---
title: "RollArt: Scaling Agentic RL Training via Disaggregated Infrastructure"
collection: publications
category: conf
permalink: /publication/rollart
excerpt: 'Wei Gao\*, Yuheng Zhao\*, <u>Tianyuan Wu</u>\*, Shaopan Xiong\*, Weixun Wang\*, Dakai An, Lunxi Cao, Dilxat Muhtar, Zichen Liu, Haizhou Zhao, Ju Huang, Siran Yang, Yongbin Li, Wenbo Su, Jiamang Wang, Lin Qu, Bo Zheng, Wei Wang (* Equal contribution).'
date: 2025-12-12
venue: 'USENIX OSDI’26'
paperurl: 'https://arxiv.org/abs/2512.22560'
# citation: 'Wei Gao*, Yuheng Zhao*, Tianyuan Wu*, Shaopan Xiong*, Weixun Wang*, Dakai An, Lunxi Cao, Dilxat Muhtar, Zichen Liu, Haizhou Zhao, Ju Huang, Siran Yang, Yongbin Li, Wenbo Su, Jiamang Wang, Lin Qu, Bo Zheng, Wei Wang., "RollArt: Scaling Agentic RL Training via Disaggregated Infrastructure", arXiv preprint arXiv:2512.22560 (2025). (*Equal contribution)'
---

Agentic Reinforcement Learning (RL) trains LLMs through multi-turn interactions with environments, producing workloads that mix compute-bound prefill, bandwidth-bound decoding, CPU-heavy environment execution, and bursty reward evaluation. Existing systems either colocate all stages on a single GPU cluster or decouple them only at a coarse granularity, overlooking hardware heterogeneity and incurring substantial synchronization overhead across stages. We present RollArt, a system for multi-task agentic RL on disaggregated infrastructure. RollArt maps each pipeline stage to best-fit hardware, routing prefill-heavy tasks to computeoptimized GPUs, decode-heavy tasks to bandwidth-optimized GPUs, and environments to CPU clusters. It decouples rollout at the trajectory level, allowing generation, environment interaction, and reward scoring to proceed independently, so that slow or failed environments never block the others. RollArt offloads stateless reward computation to serverless infrastructure and overlaps rollout with training via staleness-bounded asynchronous weight synchronization. Our results demonstrate that RollArt effectively improves training throughput and achieves 1.35–2.05× training time reduction compared to various RL systems. We also evaluate RollArt by training an MoE LLM on a cluster of over 3,000 GPUs for one week.