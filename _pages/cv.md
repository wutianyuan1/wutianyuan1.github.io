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
* Ph.D in Computer Science, Hong Kong University of Science and Technology, 2028 (expected)
* B.S. in Computer Science, ShanghaiTech University, 2021

Work experience
======
* **November 2023 - Present:** Research Intern at [Alibaba Group](https://www.alibabagroup.com/en-US/), Hangzhou, China
  * Designed and implemented a straggler detection and mitigation framework for hybrid-parallel large model training.
  * Analyzed production traces from the Alibaba HPAI cluster.
  * Mentor: [Yinghao Yu](https://scholar.google.com/citations?user=_YgjRn0AAAAJ&hl=en&oi=ao)

* **May 2022 - July 2023:** Research Intern at [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/), Beijing, China
  * Developed Catur, a NUMA-aware scheduler for VM allocation on Microsoft Azure utilizing reinforcement learning.
  * Implemented system optimizations for reinforcement learning frameworks.
  * Mentors: [Qi Chen](https://www.microsoft.com/en-us/research/people/cheqi/), [Hui Xue](https://www.microsoft.com/en-us/research/people/xuehui/)

* **August 2021 - April 2022:** Teaching Assistant at NYU Shanghai, Shanghai, China
  * Served as a teaching assistant for [CSCISHU 11 - Introduction to Computer Programming](https://bulletins.nyu.edu/courses/csci_shu/) in Fall 2021.
  * Served as a teaching assistant for [CSCISHU 2314 - Discrete Mathematics](https://shanghai.nyu.edu/academics/majors/computer-science) in Spring 2022.
  
Skills
======
- Programming Languages (in order of familiarity)
  * Python
  * C/C++
  * CUDA
  * Rust
  * Shell
  * JavaScript

- HPC/OS-related Software (in order of familiarity)
  * Linux (Ubuntu, Debian, CentOS, Arch Linux, Manjaro)
  * Docker
  * Kubernetes
  * Slurm
  * MPI, OpenMP

- DL-related Frameworks (in order of familiarity)
  * PyTorch
  * Megatron-LM
  * vLLM
  * DeepSpeed
  * Ray RLlib

- Misc
  * LaTeX
  * Markdown
  * HTML

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
