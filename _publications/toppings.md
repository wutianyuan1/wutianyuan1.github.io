---
title: "Toppings: CPU-Assisted, Rank-Aware Adapter Serving for LLM Inference"
collection: publications
category: conf
permalink: /publication/caraserve
excerpt: 'Suyi Li\*, Hanfeng Lu\*, <u>Tianyuan Wu</u>, Minchen Yu, Qizhen Weng, Xusheng Chen, Yizhou Shan, Binhang Yuan, Wei Wang (\* Equal contribution).'
date: 2025-04-25
venue: '2025 USENIX Annual Technical Conference (USENIX ATC 25)'
paperurl: 'http://www.tianyuanwu.com/files/2401.11240v1.pdf'
citation: 'Suyi Li, Hanfeng Lu, Tianyuan Wu, Minchen Yu, Qizhen Weng, Xusheng Chen, Yizhou Shan, Binhang Yuan, and Wei Wang. "CaraServe: CPU-Assisted and Rank-Aware LoRA Serving for Generative LLM Inference." arXiv preprint arXiv:2401.11240 (2024).'
---

Low-Rank Adaptation (LoRA) is a popular approach that adapts a base large language model (LLM) to domain-specific tasks by adding lightweight trainable adapters. In this paper, we present Toppings, a system that efficiently serves many LoRA adapters derived from a common base model. Toppings pins the base model on GPUs and dynamically loads the requested LoRA adapters from host memory as new requests arrive. In view of the high GPU loading overhead, which not only delays the time-to-first-token of the newly arrived request but also interrupts the ongoing decoding of all inflight queries when continuous batching is in use, Toppings proposes a CPU-assisted LoRA serving approach. It simultaneously uses CPUs to compute the lightweight adaption for prefilling as the requested LoRA adapter is being loaded onto GPUs; it then switches to the GPUs after loading completes to resume the remaining computation. Toppings develops a highly optimized synchronization mechanism and pipeline loading scheme to efficiently coordinate LoRA computation on the CPUs and GPUs. Toppings further designs a rank-aware scheduling algorithm that optimally schedules heterogeneous LoRA requests to maximize the SLO attainment. Compared with the state-of-the-art LoRA serving systems, Toppings improves the average request serving latency by up to 
1.7x and achieves an SLO attainment of up to 99%.