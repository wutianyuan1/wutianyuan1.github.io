---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Computer Science**, The Hong Kong University of Science and Technology, 2024 - 2027 (Expected)
  * CGPA: 3.98/4.30, Advisor: [Prof. Wei Wang](https://www.cse.ust.hk/~weiwa/)
* **B.S. in Computer Science**, ShanghaiTech University, 2017 - 2021
  * GPA: 3.79/4.00, Ranking: 2/209 (Top 1%)

Research Overview
======
My research focuses on building reliable and efficient infrastructure for large-scale and agentic AI systems. I have published several papers on top-tier conferences including **OSDI (x3), NSDI (x2), USENIX ATC (x2), and MLSys (x1)**. I am the awardee of the **NSDI'26 Best Paper Award**. My work spans three main areas:

**Reliable Training Infrastructure.** I develop systems that ensure robustness and efficiency in distributed training. This includes checkpointing for fault-tolerance (Portus), fail-slow detection and mitigation (Greyhound), straggler-resilient pipeline parallelism (PipeMorph), and scalable RL post-training frameworks (ROLL, AReaL-Hex, RollArt).

**Intelligent Scheduling.** I design adaptive schedulers that optimize resource utilization across diverse workloads. My contributions include time-multiplexing RL post-training jobs (Weave), long-tail rollout mitigation (RollPacker), RL-based NUMA placement for cloud VMs (Catur), and efficient LoRA adapter serving (Toppings).

**OS Support for Autonomous Agents.** I explore agent-aware operating system design that enables efficient and reliable AI agent execution (Crab), including sandboxing, resource isolation, checkpointing, memory management, and system-level orchestration techniques for agentic workloads.

Experience
======
* **October 2023 - Present:** Research Intern at [Alibaba Group](https://www.alibabagroup.com/en-US/), Hangzhou, China
  * Led the development of Greyhound, a fail-slow detection and mitigation system deployed in production clusters, achieving 1.58x improvement in end-to-end throughput for hybrid-parallel training at scale.
  * Built PipeMorph, a straggler-resilient pipeline parallelism training framework that dynamically adapts to communication stragglers, improving iteration time by 1.2-3.5x for large language models.
  * Led the design of Weave, a phase-level multi-tenant scheduler for disaggregated RL post-training that improves cost efficiency by 1.84x through fine-grained resource multiplexing.
  * Led the design of Crab, an eBPF-driven checkpoint and restore system for sandboxed AI agents that bridges the agent-OS semantics gap, reducing checkpoint frequency by 75%+ while preserving 100% correctness.
  * Co-designed the scheduling algorithm for Toppings, a CPU-assisted LoRA serving system that achieves 1.7x shorter serving latency and 99% SLO attainment.
  * Contributed to ROLL, an open-source RL post-training framework, and co-led the development of RollArt, a disaggregated infrastructure achieving 1.35-2.05x speedup for agentic RL training. Also contributed to RollPacker, which reduces end-to-end training time by 2.03-2.56x in synchronous RL post-training.
  * Analyzed large-scale production traces from Alibaba clusters to understand GPU utilization characteristics and reliability issues in the era of generative AI.

* **May 2022 - July 2023:** Research Intern at [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/), Beijing, China
  * Developed Catur, an RL-based virtual NUMA placement system for Microsoft Azure. Successfully verified and deployed on Hyper-V, it reduces remote memory accesses by 75.2% for diverse VM workloads.
  * Won the "Stars of the Future" award for outstanding research contributions (top 10% of interns).

* **August 2021 - May 2022:** Teaching Assistant at [NYU Shanghai](https://shanghai.nyu.edu/), Shanghai, China
  * Designed assignments and led discussions for Discrete Mathematics and Computer Programming courses.
  * Developed an automated grading system for programming assignments, serving 200+ students.

* **July 2020 - October 2020:** Research Intern at [Institute of Computing Technology, Chinese Academy of Sciences](http://www.ict.ac.cn/), Beijing, China
  * Built a memory access pattern analyzer using the ROSE compiler infrastructure, enabling automated classification of complex access patterns and informing prefetcher design.

Awards
======
* NSDI'26 Best Paper Award, USENIX Association, 2026.
* Research Travel Grant, HKUST, 2025.
* Enhanced Redbird PhD Award, HKUST, 2024 and 2025.
* Post-graduate Scholarship, HKUST, 2024.
* Stars of the Future, Microsoft Research, 2023.
* Outstanding Undergraduate Thesis, ShanghaiTech University, 2021.
* Outstanding Teaching Assistant Award, ShanghaiTech University, 2019, 2020, and 2021.
* Second-class Scholarship, ShanghaiTech University, 2019.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
