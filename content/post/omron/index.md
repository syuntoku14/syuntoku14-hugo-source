---
title: OMRON SINIC X (OSX) のインターン感想

# Link this post with a project
projects: []

# Date published
date: "2022-02-25T00:00:00Z"

# Date updated
lastmod: "2022-02-25T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Research
- Internship

categories:
- Internship
---

2021年6月から2022年2月まで, [オムロンサイニックエックス (OSX)](https://www.omron.com/sinicx/) にて研究インターンをさせていただきました. 
これはOSXインターンについてまとめたポストになります.
元インターンの[奥村さんのポスト](https://kei18.github.io/posts/20211129_osx-intern.html)も参考になるのでぜひ.

## 自己紹介

* 現在は奈良先端科学技術大学院大学の修士２年, 2022年の4月から東京大学で博士課程に進学予定の学生です.
* 学部の頃はロボットよりの研究をしていましたが, 修士課程では強化学習の理論やアルゴリズムがメインの研究をやっていました. 
* 詳しくは[ホームページ](https://syuntoku14.github.io/)を見てね.

## インターンまでの経緯

M2の前半で主著を1つ & 共著を2つ生やすことができたので, M2の後半はインターンやりたいなあ〜って思っていたところ, 研究室経由でメンターの[米谷さん](https://yonetaniryo.github.io/)からOSXインターンのお誘いをいただきました.
待遇や時期的にもかなり好条件だったので即返事をし, フルタイムで半年以上の研究インターンに参加させていただきました.
インターンへの応募は[ここ](https://medium.com/sinicx/fy2021-%E7%A0%94%E7%A9%B6%E3%82%A4%E3%83%B3%E3%82%BF%E3%83%BC%E3%83%B3%E3%81%AE%E5%8B%9F%E9%9B%86-fd6cc05e8098)に詳細があります.

## 何をやったのか

強化学習の理論と応用の実験をサポートしたライブラリ [ShinRL](https://github.com/omron-sinicx/ShinRL) を開発しました.
当初は米谷さんの提案でオフライン強化学習のテーマに取り組んでおり, 僕が個人的に開発していたShinRLを使ってデバッグ & アルゴリズムの実装を進めていました.
もっとShinRLを高速化したい, 実装をキレイにしたい, などの理由で途中からShinRLの開発にシフトし始め, 最終的にはOSXとしてオフィシャルに公開するのを目標にテーマを変更しました (米谷さんは快く承諾していただきました. 圧倒的感謝).

当初はPyTorchで実装していたShinRLですが, 速度面や実装の単純さ, 勉強目的からJAXを利用して実装することに (米谷さんとJAXの勉強ができて楽しかったです).

