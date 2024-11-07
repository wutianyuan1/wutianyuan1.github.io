---
title: "CaraServe: CPU-Assisted and Rank-Aware LoRA Serving for Generative LLM Inference"
collection: publications
category: preprints
permalink: /publication/caraserve
excerpt: 'Suyi Li\*, Hanfeng Lu\*, <u>TTianyuan Wu</u>, Minchen Yu, Qizhen Weng, Xusheng Chen, Yizhou Shan, Binhang Yuan, Wei Wang (\* Equal contribution).'
date: 2024-01-15
venue: 'Arxiv Preprint'
paperurl: 'http://www.tianyuanwu.com/files/2401.11240v1.pdf'
citation: 'Suyi Li, Hanfeng Lu, Tianyuan Wu, Minchen Yu, Qizhen Weng, Xusheng Chen, Yizhou Shan, Binhang Yuan, and Wei Wang. "CaraServe: CPU-Assisted and Rank-Aware LoRA Serving for Generative LLM Inference." arXiv preprint arXiv:2401.11240 (2024).'
---

Pre-trained large language models (LLMs) often need specialization for domain-specific tasks. Low-Rank Adaptation (LoRA) is a popular approach that adapts a base model to multiple tasks by adding lightweight trainable adapters. In this paper, we present CaraServe, a system that efficiently serves many LoRA adapters derived from a common base model. CaraServe maintains the base model on GPUs and dynamically loads activated LoRA adapters from main memory. As GPU loading results in a cold-start that substantially delays token generation, CaraServe employs a CPU-assisted approach. It early starts the activated adapters on CPUs for prefilling as they are being loaded onto GPUs; after loading completes, it then switches to the GPUs for generative LoRA inference. CaraServe develops a highly optimized synchronization mechanism to efficiently coordinate LoRA computation on the CPU and GPU. Moreover, CaraServe employs a rank-aware scheduling algorithm to optimally schedule heterogeneous LoRA requests for maximum service-level objective (SLO) attainment. We have implemented CaraServe and evaluated it against state-of-the-art LoRA serving systems. Our results demonstrate that CaraServe can speed up the average request serving latency by up to 1.4x and achieve an SLO attainment of up to 99%.