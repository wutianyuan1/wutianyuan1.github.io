---
title: "Portus: Efficient DNN Checkpointing to Persistent Memory with Zero-Copy"
collection: publications
category: conf
permalink: /publication/portus
excerpt: 'Yuanhao Li\*, <u>Tianyuan Wu*</u>, Guancheng Li, Yanjie Song, Shu Yin (\* Equal contribution).'
date: 2024-07-23
venue: '44th IEEE International Conference on Distributed Computing Systems (ICDCS\'24)'
paperurl: 'http://www.tianyuanwu.com/files/portus.pdf'
citation: 'Li, Yuanhao, Tianyuan Wu, Guancheng Li, Yanjie Song, and Shu Yin. "Portus: Efficient DNN Checkpointing to Persistent Memory with Zero-Copy." In 2024 IEEE 44th International Conference on Distributed Computing Systems (ICDCS), pp. 59-70. IEEE, 2024.'
---

We introduce Portus, an efficient checkpointing system for DNN models. The core of Portus is a three-level index structure and a direct RDMA datapath that enables fast check-points between GPUs and persistent memory in a serialization-free way. Portus offers a zero-copy approach between GPU and persistent memory without involving main memory and kernel crossings to underlying file systems. Portus also applies an asynchronous mechanism to hide the checkpointing overhead in the model training procedures. We integrated a Portus prototype into a high-performance AI cluster with NVIDIA®V100 and A40 GPUs and Intel®Optane™persistent memory, then evaluated its performance in both single-GPU and multi-GPU large model training scenarios. Experiment results show that compared to a state-of-the-art checkpointing system, Portus achieves up to 9.23× and 7.0× speedup in checkpointing and restoring, respectively. Portus achieves up to 2.6× higher throughput and 8× faster checkpointing operation on a large language model, GPT-22B.