---
title: "FALCON: Pinpointing and Mitigating Stragglers for Large-Scale Hybrid-Parallel Training"
collection: publications
category: preprints
permalink: /publication/falcon
excerpt: '<u>Tianyuan Wu</u>, Wei Wang, Yinghao Yu, Siran Yang, Wenchao Wu, Qinkai Duan, Guodong Yang, Jiamang Wang, Lin Qu, Liping Zhang.'
date: 2024-09-18
venue: 'Arxiv Preprint'
paperurl: 'http://www.tianyuanwu.com/files/2410.12588v1.pdf'
citation: 'Tianyuan Wu, Wei Wang, Yinghao Yu, Siran Yang, Wenchao Wu, Qinkai Duan, Guodong Yang, Jiamang Wang, Lin Qu, and Liping Zhang. "FALCON: Pinpointing and Mitigating Stragglers for Large-Scale Hybrid-Parallel Training." arXiv preprint arXiv:2410.12588 (2024).'
---

Fail-slows, or stragglers, are common but largely unheeded problems in large-scale hybrid-parallel training that spans thousands of GPU servers and runs for weeks to months. Yet, these problems are not well studied, nor can they be quickly detected and effectively mitigated. In this paper, we first present a characterization study on a shared production cluster with over 10,000 GPUs1. We find that fail-slows are caused by various CPU/GPU computation and cross-node networking issues, lasting from tens of seconds to nearly ten hours, and collectively delaying the average job completion time by 1.34%. The current practice is to manually detect these fail-slows and simply treat them as fail-stops using a checkpoint-and-restart failover approach, which are labor-intensive and time-consuming. In this paper, we propose FALCON, a framework that rapidly identifies fail-slowed GPUs and/or communication links, and effectively tackles them with a novel multi-level mitigation mechanism, all without human intervention. We have applied FALCON to detect human-labeled fail-slows in a production cluster with over 99% accuracy. Cluster deployment further demonstrates that FALCON effectively handles manually injected fail-slows, mitigating the training slowdown by 60.1%.
