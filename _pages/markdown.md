---
permalink: /markdown/
title: "Misc"
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---

## Madoka's Playlist - 2025

* 粼粼 - 银临
* 流光记 - 银临
* 腐草为萤 - 银临
* 牵丝戏 - 银临
* 锦鯉抄 - 银临
* 棠梨煎雪 - 银临
* 小さな恋のうた - 小さな恋のうた
* 藍悼花 (feat. Lucia) - 酔シグレ
* 花簧り - 滴草由実
* 春江花月夜 - 祖娅纳惜

## Madoka's Playlist - 2024
* 変わらないもの - 奥華子
* Siawase - 鎖那
* ハロ／ハワユ - 初音ミク
* 願い～あの頃のキミへ～ - 當山みれい
* La vaguelette - HOYO MIX
* POWDER SNOW - 水樹奈々
* 届かない恋 - 茅野愛衣
* WHITE ALBUM - 小木曽雪菜
* My Soul, Your Beats! - Lia
* 砕月 - 東方萃夢想

## Learn to Become a Good Researcher
```c++
std::future<void> 
Researcher<CS>::week(std::shared_ptr<Paper> paper) {
  return std::async(std::launch::async, [this, paper]() -> std::future<void> {
      try {
          auto thoughts = paper->read_and_digest().get();
          auto progress = this->project->coding().get();
          auto compiled = compile(thoughts, progress);
          return this->meeting->report(compiled);
      } catch (const std::exception& e) {
          std::cerr << "Never gives up on " << e.what() << std::endl;
          return this->week(paper);
      }
  });
}
```
(Idea by [Jose Hu](https://www.josehu.com/))
