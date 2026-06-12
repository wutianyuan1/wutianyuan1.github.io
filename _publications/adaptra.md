---
title: "Attack of the Bubbles: Straggler-Resilient Pipeline Parallelism for Large Model Training"
collection: publications
category: conf
permalink: /publication/adaptra
badge: 'NSDI 26'
award: 'Best Paper Award'
excerpt: '<u>Tianyuan Wu*</u>, Lunxi Cao\*, Hanfeng Lu, Xiaoxiao Jiang, Yinghao Yu, Siran Yang, Guodong Yang, Jiamang Wang, Lin Qu, Liping Zhang, Wei Wang (\* Equal contribution).'
date: 2025-07-14
venue: 'USENIX Symposium on Networked Systems Design and Implementation (NSDI), Renton, May 2026.'
paperurl: 'http://wutianyuan1.github.io/files/nsdi26spring-final218.pdf'
slidesurl: 'http://wutianyuan1.github.io/files/pipemorph_sim'
---

Training large Deep Neural Network (DNN) models at scale often encounters straggler issues, mostly in communications due to network congestion, RNIC/switch defects, or topological asymmetry. Under advanced pipeline parallelism, even minor communication delays can induce significant training slowdowns. This occurs because (1) slow communication disrupts the pipeline schedule, creating cascading "bubbles" in a domino effect, and (2) current GPU kernel scheduling is susceptible to head-of-line blocking, where slow communication blocks subsequent computations, further adding to these bubbles. To address these challenges, we present PipeMorph, a straggler-resilient training system with two key optimizations. First, it optimally adapts the pipeline schedule in the presence of stragglers to absorb communication delays without inducing cascading bubbles, using a simple yet effective algorithm guided by an analytical model. Second, upon detecting slow communication, PipeMorph offloads communication operations from GPU to host memory and utilizes CPU-side RDMA for data transfer. This eliminates head-of-line blocking as subsequent computation kernels can be scheduled immediately on GPUs. Together, these optimizations effectively reduce pipeline stalls in the presence of communication stragglers, improving the training iteration time by 1.2-3.5x in our experiments under various settings.
