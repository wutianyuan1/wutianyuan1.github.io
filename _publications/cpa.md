---
title: "CPA: Efficient and Stable FP4 RL Training via Cross-Precision Alignment"
collection: publications
category: conf
permalink: /publication/cpa
badge: 'NeurIPS 26'
excerpt: 'Gu Gong*, Yining Wei*, Yuechen Tao, <u>Tianyuan Wu</u>, Peijie Dong, Ruibo Fan, Wenhu Hu, Yinghao Yu, Jiamang Wang, Wenbo Su, Guodong Yang, Liping Zhang, Wei Wang, Xiaowen Chu (* Equal contribution).'
date: 2026-09-25
venue: 'Conference on Neural Information Processing Systems (NeurIPS), 2026. Poster.'
paperurl: 'https://wutianyuan1.github.io/files/NeurIPS26_CPA.pdf'
---

Reinforcement learning (RL) for large language models is increasingly bottlenecked by rollout cost, making low-precision rollout appealing for acceleration. However, FP4 quantization amplifies small numerical differences between training and inference into large token-level log-probability errors, destabilizing optimization. Cross-Precision Alignment (CPA) stabilizes low-precision RL by maintaining a BF16 master policy, executing rollouts in real FP4, and aligning the fake-quantized forward pass with a BF16 reference through a low-variance KL penalty on sampled tokens. The resulting BF16 checkpoint matches a full BF16 RL baseline while the overall pipeline delivers 8–19% end-to-end training speedup.
