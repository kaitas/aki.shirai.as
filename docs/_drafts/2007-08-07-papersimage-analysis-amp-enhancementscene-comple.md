---
author: ameblo
title: "\n\t\t\t\tPapers/Image Analysis &amp; Enhancement/Scene Comple\t\t"
slug: papersimage-analysis-amp-enhancementscene-comple
id: 3323
date: '2007-08-07 05:01:12'
layout: post
categories:
  - SIGGRAPH
---

スタバでコーヒーかってPaperでセッション聞きながらたまったメールとかを処理中。 セッションはPapers「Image Analysis & Enhancement」。 この分野は最近発展が目覚しいよな。 とりあえず使い道があるかわからないので、眺めているだけなんだけど。 ”Scene Completion Using Millions of Photographs” (James Hays, CMU) [http://graphics.cs.cmu.edu/projects/scene-completion/](http://graphics.cs.cmu.edu/projects/scene-completion/) 風景画像中の任意のエリアを切り取って、別の画像から適切な写真を自然に張り込む。 結果だけ見ているとまるで魔法。 2.3百万の画像をFlickrからダウンロードしてデータベースを作っているらしい。 候補は200ぐらいでている。 実際には元になっているスナップ写真ではなくて、まったく同じ場所の別の写真などから張り込まれていることもあるようだ。 評価もちゃんとやっていて、提案手法は0.6の割合でFakeと認識されるらしい。 ちなみに実際の写真は0.1、Criminisiらの手法は0.9。