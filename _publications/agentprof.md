---
title: "AgentProf: Semantic Profiling for AI Agents"
collection: publications
category: conf
permalink: /publication/agentprof
badge: 'AgenticOS 26'
excerpt: 'Yusheng Zheng, Chaokun Chang, <u>Tianyuan Wu</u>, Wenan Mao, Shuyi Cheng, Tao Ma, Andi Quinn, Wei Wang.'
date: 2026-09-03
venue: "AgenticOS '26, 2026."
paperurl: 'https://wutianyuan1.github.io/files/agenticos26-paper27.pdf'
---

AI agents increasingly orchestrate long-running, multi-step activities involving thousands to millions of interactions with users, tools, and system resources. To improve quality, safety, and cost efficiency, developers need to determine where failures concentrate, which workflows trigger unsafe effects, and which task categories consume the most budget. AgentProf introduces a semantic operation stack model that adapts profiling to agent trajectories. Uniform operations represent all agent activities, and operation stacks replace the runtime call stack, enabling hierarchical attribution at different levels of granularity from the same data. AgentProf implements this model as an offline profiler with pluggable algorithms for intent attribution and stack construction, compiling local agent trajectories into pprof-compatible profiles.
