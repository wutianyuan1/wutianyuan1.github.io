---
title: "Greyhound: Hunting Fail-Slows in Hybrid-Parallel Training at Scale"
collection: publications
category: conf
permalink: /publication/greyhound
excerpt: '<u>Tianyuan Wu</u>, Wei Wang, Yinghao Yu, Siran Yang, Wenchao Wu, Qinkai Duan, Guodong Yang, Jiamang Wang, Lin Qu, Liping Zhang.'
date: 2025-04-25
venue: '2025 USENIX Annual Technical Conference (USENIX ATC 25)'
paperurl: 'http://www.tianyuanwu.com/files/atc25-wu-tianyuan.pdf'
citation: 'Tianyuan Wu, Wei Wang, Yinghao Yu, Siran Yang, Wenchao Wu, Qinkai Duan, Guodong Yang, Jiamang Wang, Lin Qu, and Liping Zhang, ‘‘Greyhound: Hunting Fail-Slows in Hybrid-Parallel Training at Scale,’’ in the Proceedings of USENIX Annual Technical Conference (ATC ’25), Boston, MA, USA, July 2025.'
---

[Presentation slides](http://www.tianyuanwu.com/files/ATC25_greyhound_presentation.pdf)

Fail-slows, or stragglers, are common problems in large-scale hybrid-parallel training that runs on a large fleet of GPU servers for an extended period of time. Yet, these problems are not well studied. In this paper, we first present a characterization study on a shared production cluster with over 10,000 GPUs. We find that fail-slows manifest as transient stragglers caused by slow computations or communications due to contention, device degradation, or network congestion, lasting from sub-minutes to nearly ten hours, and delaying large training jobs by 1.34× on average. The current practice is to manually detect fail-slows and treat them as fail-stops by means of checkpoint-and-restart failover, which is time-consuming. In this paper, we propose GREYHOUND, a system that rapidly identifies slow GPUs and/or communication links, and effectively tackles them with a novel multi-level mitigation mechanism, all without human intervention. GREYHOUND correctly detects fail-slows in a production cluster with over 99% accuracy. Testbed experiment on 256 H800 GPUs further demonstrates that it effectively handles (manually injected) stragglers, mitigating the slowdown by 58.9%.
