---
title: "Virtual Machine NUMA Placement at Scale: Learning the Norm, Shielding the Tail"
collection: publications
category: conf
permalink: /publication/catur
badge: 'MLSys 26'
excerpt: 'Yibo Zhao\*, <u>Tianyuan Wu*</u>, Hui Xue, Qi Chen, Zhenhua Han, Zikai Xu, Yuntai Chang, Rui Gao, Steve Deng, Ray Jui-Hao Chiang, Mingxia Li, Yuqing Yang, Cheng Tan, Fan Yang, Peng Cheng, Yongqiang Xiong, Lili Qiu, Lidong Zhou (\* Equal contribution).'
date: 2025-07-14
venue: 'Annual Conference on Machine Learning and Systems (MLSys), Bellevue, May 2026.'
paperurl: 'https://openreview.net/forum?id=guCUThRvX5'
---

In modern data centers, servers organize memory and CPUs into Non-Uniform Memory Access (NUMA) nodes, where unequal memory-to-CPU proximity leads to varying memory latency. Hypervisors must carefully place Virtual Machines (VMs) to reduce remote memory access. Poor placements can lead to significant performance degradation—sometimes up to 30%. However, achieving optimal placement at scale is challenging due to the large number of VM configurations, diverse NUMA structures, and evolving workload patterns. We present Catur, a NUMA placement system designed for large-scale cloud environments. Catur leverages reinforcement learning to learn from production data. Moreover, to address real-world challenges, Catur integrates several techniques: robust action space design to prevent model collapse, reward shaping to address learning inefficiency, drift-aware continuous training for evolving workload patterns, and speculative shielding to mitigate VM performance anomalies. Evaluations on production traces with 100 million VMs demonstrate that Catur reduces average resource defect by 34.2%-50.0% compared to state-of-the-art hypervisor policies.
