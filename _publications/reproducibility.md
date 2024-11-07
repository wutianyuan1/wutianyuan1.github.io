---
title: "Reproducibility: Performance Evaluation of MemXCT on Azure CycleCloud Platform"
collection: publications
category: manuscripts
permalink: /publication/reproducibility
excerpt: 'Yuchen Liu\*, Yixuan Meng\*, Kaiyuan Xu\*, Zijun Xu\*, <u>Tianyuan Wu\*</u>, Yiwei Yang\*, Shu Yin\* (\* All authors contributed equally).'
date: 2021-11-11
venue: 'IEEE Transactions on Parallel and Distributed Systems, 2021'
paperurl: 'http://www.tianyuanwu.com/files/reproducibility.pdf'
citation: 'Yuchen Liu, Yixuan Meng, Kaiyuan Xu, Zijun Xu, Tianyuan Wu, Yiwei Yang, and Shu Yin. "Reproducibility: Performance Evaluation of MemXCT on Azure CycleCloud Platform." IEEE Transactions on Parallel and Distributed Systems 33, no. 9 (2021): 2047-2049.'
---

Memory-Centric X-ray Computational Tomography(CT) is an iterative reconstruction technique that trades compute simplifications with higher memory accesses. MemXCT implements a sparse matrix-vector multiplication(SpMV) with multi-stage buffering and two-level pseudo-Hilbert ordering for optimization. Motivated by the need to validate conclusions from previous work, we reproduce the numerical results, the algorithm’s performance, and the scaling behavior of the algorithms as the number of MPI processes increases on Azure.