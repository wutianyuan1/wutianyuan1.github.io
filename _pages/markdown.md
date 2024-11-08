---
permalink: /markdown/
title: "Misc"
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---

## Madoka's Playlist
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