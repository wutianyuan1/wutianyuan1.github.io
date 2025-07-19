---
title: "Adaptra: Straggler-Resilient Hybrid-Parallel Training with Pipeline Adaptation"
collection: publications
category: preprints
permalink: /publication/adaptra
excerpt: '<u>Tianyuan Wu*</u>, Lunxi Cao*, Hangeng Lu, Xiaoxiao Jiang, Yinghao Yu, Siran Yang, Guodong Yang, Jiamang Wang, Lin Qu, Liping Zhang, Wei Wang.'
date: 2025-05-01
venue: 'arXiv preprint'
paperurl: 'http://www.tianyuanwu.com/files/2504.19232v1.pdf'
citation: 'Tianyuan Wu*, Lunxi Cao*, Hanfeng Lu, Xiaoxiao Jiang, Yinghao Yu, Siran Yang, Guodong Yang, Jiamang Wang, Lin Qu, Liping Zhang, and Wei Wang, "Attack of the Bubbles: Straggler-Resilient Pipeline Parallelism for Large Model Training," in the Proceedings of the 23rd USENIX Symposium on Networked Systems Design and Implementation (NSDI ’26), Renton, WA, USA, May 2026. (*Equal contribution)'
---

Training large Deep Neural Network (DNN) models at scale often encounters straggler issues, mostly in communications due to network congestion, RNIC/switch defects, or
topological asymmetry. Under advanced pipeline parallelism,
even minor communication delays can induce significant training slowdowns. This occurs because (1) slow communication
disrupts the pipeline schedule, creating cascading “bubbles”
in a domino effect, and (2) current GPU kernel scheduling is
susceptible to head-of-line blocking, where slow communication blocks subsequent computations, further adding to these
bubbles. To address these challenges, we present ADAPTRA, a
straggler-resilient training system with two key optimizations.
First, it optimally adapts the pipeline schedule in the presence
of stragglers to absorb communication delays without inducing cascading bubbles, using a simple yet effective algorithm
guided by an analytical model. Second, upon detecting slow
communication, ADAPTRA offloads communication opera-
tions from GPU to host memory and utilizes CPU-side RDMA
for data transfer. This eliminates head-of-line blocking as subsequent computation kernels can be scheduled immediately
on GPUs. Together, these optimizations effectively reduce
pipeline stalls in the presence of communication stragglers,
improving the training iteration time by 1.2-3.5×in our experiments under various settings