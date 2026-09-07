---
permalink: /zh/
title: "关于我"
author_profile: true
author: tianyuan_zh
lang: zh-CN
alternate_lang: en-US
alternate_url: /
description: "吴天元"
---

我是[香港科技大学（HKUST）](https://hkust.edu.hk/)计算机科学与工程系博士生，有幸师从[王威教授](https://www.cse.ust.hk/~weiwa/)。

我的研究方向是机器学习系统，主要关注面向大规模训练的可靠系统框架，同时也在探索强化学习与智能体系统。攻读博士学位前，我于 2021 年获得[上海科技大学](https://www.shanghaitech.edu.cn/)信息科学与技术学院工学学士学位，随后在[微软亚洲研究院](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/)系统组实习，并获得“明日之星”奖。我曾获得 NSDI'26 最佳论文奖，并在 OSDI、NSDI、USENIX ATC 等顶级会议发表多篇论文。

我希望生活不止于代码和系统，也能真切地感受每一天。徒步穿越青藏高原时体会的深沉寂静，以及[那些令人动容的旋律](https://wutianyuan1.github.io/markdown/)带来的情感共鸣，都提醒着我：生命短暂而偶有忧伤，其意义并不只在终点，更在于旅途本身的丰盈。

邮箱：twubt [at] connect [dot] ust [dot] hk

<div class="home-columns" markdown="1">
<section class="home-column" markdown="1">

最新动态
======
- [09/2026] [AgentProf](http://wutianyuan1.github.io/files/agenticos26-paper27.pdf) 将发表于 AgenticOS'26。
- [09/2026] [Moye](https://wutianyuan1.github.io/files/sc26-echo.pdf) 将发表于 [SC'26](https://sc26.supercomputing.org/)。
- [05/2026] [Crab](https://arxiv.org/abs/2604.28138) 已上线 arXiv。
- [05/2026] [PipeMorph](http://wutianyuan1.github.io/files/2504.19232v1.pdf) 获得 [NSDI'26](https://www.usenix.org/conference/nsdi26/) 最佳论文奖。
- [04/2026] 三篇论文（[Weave](https://arxiv.org/abs/2512.11306v1)、[RollArt](https://arxiv.org/abs/2512.22560) 和 [ASI Trace Analysis](https://www.usenix.org/conference/osdi26)）被 [OSDI'26](https://www.usenix.org/conference/osdi26) 接收。
- [01/2026] [Catur](https://openreview.net/forum?id=guCUThRvX5) 被 [MLSys'26](https://mlsys.org/Conferences/2026) 接收。
- [12/2025] [Weave](https://arxiv.org/abs/2512.11306v1) 和 [RollArt](https://arxiv.org/abs/2512.22560) 已上线 arXiv。
- [12/2025] [RollPacker](https://arxiv.org/abs/2509.21009) 被 [NSDI'26](https://www.usenix.org/conference/nsdi26/) 接收。
- [11/2025] 求购 2026 年 2 月 22 日在日本横滨举办的《白色相簿 2》音乐会门票。
- [11/2025] 三篇强化学习相关论文 [ROLL](https://arxiv.org/abs/2506.06122)、[RollPacker](https://arxiv.org/abs/2509.21009) 和 [AReaL-Hex](https://arxiv.org/abs/2511.00796) 已上线 arXiv。
- [07/2025] [PipeMorph](http://wutianyuan1.github.io/files/2504.19232v1.pdf) 被 [NSDI'26](https://www.usenix.org/conference/nsdi26/) 接收。
- [04/2025] 两篇论文（[Greyhound](http://wutianyuan1.github.io/files/atc25-wu-tianyuan.pdf) 和 [Toppings](http://wutianyuan1.github.io/files/atc25-li-suyi-toppings.pdf)）被 [USENIX ATC'25](https://www.usenix.org/conference/atc25) 接收。
- [11/2024] [RASTER](http://wutianyuan1.github.io/files/socc24-final138.pdf) 被 [ACM SoCC'24](https://acmsocc.org/2024/schedule.html) 接收。
- [06/2024] [Portus](https://www.computer.org/csdl/proceedings-article/icdcs/2024/860500a059/1ZCgEAXHPCE) 被 [ICDCS'24](https://icdcs2024.icdcs.org/) 接收。

</section>
<section class="home-column home-posts" markdown="1">

最近文章
======

{% assign recent_posts = site.categories.technical %}
{% if recent_posts and recent_posts.size > 0 %}
<ul class="home-post-list">
{% for post in recent_posts limit: 5 %}
  <li>
    <a class="home-post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
    {% if post.excerpt %}<p>{{ post.excerpt | strip_html | strip_newlines | truncate: 120 }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

[查看全部文章 →]({{ '/posts/' | relative_url }}){: .home-posts-more }
{% else %}
技术随笔即将更新。
{: .home-posts-empty }
{% endif %}

</section>
</div>
