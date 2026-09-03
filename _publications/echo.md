---
title: "Scalable and Efficient Simulation of LLM Training"
collection: publications
category: conf
permalink: /publication/echo
badge: 'SC 26'
excerpt: 'Yicheng Feng, Kin Hang Sew, Yuetao Chen, Kaiwen Chen, Jingzong Li, <u>Tianyuan Wu</u>, Zheng Zhou, Peng Cheng, Chuan Wu, Wei Wang, Tsung-Yi Ho, Hong Xu.'
date: 2026-09-03
venue: 'The International Conference for High Performance Computing, Networking, Storage, and Analysis (SC), Chicago, November 2026.'
paperurl: 'https://wutianyuan1.github.io/files/sc26-echo.pdf'
---

Simulation offers unique value for both enumeration and extrapolation and is becoming increasingly important for managing massive machine-learning clusters and large-scale distributed training jobs. Echo tackles three key challenges in large-scale training simulation: tracing runtime training workloads at each device ex situ, accurately estimating collective communication without the overhead of discrete-event network simulation, and accounting for interference-induced computation slowdown when communication and computation kernels overlap on the same device. Echo supports dense and MoE workloads with high fidelity and enables GPU-memory-aware ex-situ simulation.
