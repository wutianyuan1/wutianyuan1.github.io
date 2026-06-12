---
title: "Portus: Efficient DNN Checkpointing to Persistent Memory with Zero-Copy"
collection: publications
category: conf
permalink: /publication/portus
badge: 'ICDCS 24'
excerpt: 'Yuanhao Li*, <u>Tianyuan Wu*</u>, Guancheng Li, Yanjie Song, Shu Yin (* Equal contribution).'
date: 2024-07-23
venue: 'IEEE International Conference on Distributed Computing Systems (ICDCS), Jersey City, July 2024.'
paperurl: 'http://wutianyuan1.github.io/files/portus.pdf'
---

We introduce Portus, an efficient checkpointing system for DNN models. The core of Portus is a three-level index structure and a direct RDMA datapath that enables fast checkpoints between GPUs and persistent memory in a serialization-free way. Portus offers a zero-copy approach between GPU and persistent memory without involving main memory and kernel crossings to underlying file systems. Portus also applies an asynchronous mechanism to hide the checkpointing overhead in the model training procedures. We integrated a Portus prototype into a high-performance AI cluster with NVIDIA V100 and A40 GPUs and Intel Optane persistent memory, then evaluated its performance in both single-GPU and multi-GPU large model training scenarios. Experiment results show that compared to a state-of-the-art checkpointing system, Portus achieves up to 9.23x and 7.0x speedup in checkpointing and restoring, respectively. Portus achieves up to 2.6x higher throughput and 8x faster checkpointing operation on a large language model, GPT-22B.
