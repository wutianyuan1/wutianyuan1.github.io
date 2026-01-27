---
title: "RollArt: Scaling Agentic RL Training via Disaggregated Infrastructure"
collection: publications
category: conf
permalink: /publication/rollart
excerpt: 'Wei Gao*, Yuheng Zhao*, <u>Tianyuan Wu</u>*, Shaopan Xiong*, Weixun Wang*, Dakai An, Lunxi Cao, Dilxat Muhtar, Zichen Liu, Haizhou Zhao, Ju Huang, Siran Yang, Yongbin Li, Wenbo Su, Jiamang Wang, Lin Qu, Bo Zheng, Wei Wang.'
date: 2025-12-12
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2512.22560'
citation: 'Wei Gao*, Yuheng Zhao*, Tianyuan Wu*, Shaopan Xiong*, Weixun Wang*, Dakai An, Lunxi Cao, Dilxat Muhtar, Zichen Liu, Haizhou Zhao, Ju Huang, Siran Yang, Yongbin Li, Wenbo Su, Jiamang Wang, Lin Qu, Bo Zheng, Wei Wang., "RollArt: Scaling Agentic RL Training via Disaggregated Infrastructure", arXiv preprint arXiv:2512.22560 (2025). (*Equal contribution)'
---

Agentic Reinforcement Learning (RL) enables Large Language Models (LLMs) to perform autonomous decision-making and long-term planning. Unlike standard LLM post-training, agentic RL workloads are highly heterogeneous, combining compute-intensive prefill phases, bandwidth-bound decoding, and stateful, CPU-heavy environment simulations. We argue that efficient agentic RL training requires disaggregated infrastructure to leverage specialized, best-fit hardware. However, naive disaggregation introduces substantial synchronization overhead and resource underutilization due to the complex dependencies between stages.
We present RollArt, a distributed system designed to maximize throughput for multi-task agentic RL on disaggregated infrastructure. RollArt is built on three core principles: (1) hardware-affinity workload mapping, which routes compute-bound and bandwidth-bound tasks to bestfit GPU devices, (2) fine-grained asynchrony, which manages execution at the trajectory level to mitigate resource bubbles, and (3) statefulness-aware computation, which offloads stateless components (e.g., reward models) to serverless infrastructure for elastic scaling. Our results demonstrate that RollArt effectively improves training throughput and achieves 1.35-2.05x end-to-end training time reduction compared to monolithic and synchronous baselines. We also evaluate RollArt by training a hundreds-of-billions-parameter MoE model for Qoder product on an Alibaba cluster with more than 3,000 GPUs, further demonstrating RollArt scalability and robustness.
