---
title: "Reinforcement Learning Optimization for Large-Scale Learning: An Efficient and User-Friendly Scaling Library"
collection: publications
category: conf
permalink: /publication/roll
excerpt: 'ROLL Team.'
date: 2025-06-06
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2506.06122'
citation: 'ROLL Team, "Reinforcement Learning Optimization for Large-Scale Learning: An Efficient and User-Friendly Scaling Library", arXiv preprint arXiv:2506.06122 (2025).'
---

We introduce ROLL, an efficient, scalable, and user-friendly library designed for Reinforcement Learning Optimization for Large-scale Learning. ROLL caters to three primary user groups: tech pioneers aiming for cost-effective, fault-tolerant large-scale training, developers requiring flexible control over training workflows, and researchers seeking agile experimentation. ROLL is built upon several key modules to serve these user groups effectively. First, a single-controller architecture combined with an abstraction of the parallel worker simplifies the development of the training pipeline. Second, the parallel strategy and data transfer modules enable efficient and scalable training. Third, the rollout scheduler offers fine-grained management of each sample's lifecycle during the rollout stage. Fourth, the environment worker and reward worker support rapid and flexible experimentation with agentic RL algorithms and reward designs. Finally, AutoDeviceMapping allows users to assign resources to different models flexibly across various stages.