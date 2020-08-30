---
author: ameblo
title: "\n\t\t\t\tDromeEngine on Ubuntu\t\t"
slug: dromeengine-on-ubuntu
id: 3191
date: '2007-03-16 23:54:11'
layout: post
categories:
  - Graphics
tags:
  - 教育
---

今日は技術の話。 DromeEngineという結構昔の3Dエンジンを掘り起こしてみて、挙動やソースを確認してみたくなった。 昨日 http://www.3ddrome.com/engine.php からDromeEngine-0.3.3.tar.gzを落として、Ubuntu上でいろいろ試してみたんだけど、makeがうまくいかない（/src/gfx)。 最終更新がApril 23, 2005とかあるから無理もないのか…。 とりあえgfx_gl.cppの以下の箇所をコメントアウトすると動きます。 // set ARB_*_program function pointers if(arb_vertex_program || arb_fragment_program) { SET_FUNC_POINTER(glGenProgramsARB); SET_FUNC_POINTER(glDeleteProgramsARB); SET_FUNC_POINTER(glBindProgramARB); SET_FUNC_POINTER(glProgramStringARB); } たぶん、GLのARB拡張の関数フォーマットとかが以前と変わったからとかなんだろうけど、追いきれてません。 さて、Dromeですが、Quakeスタイルの古めのエンジンなんだけど、とりあえず上記のエラーでもわかるように頂点/ピクセルシェーダーをサポートしています。 しかし手元でコンパイルしたものは別のレベルを読み込もうとするとcoredumpしてしまう…。 まあサンプルとか作ってみてもよかったんだけどとりあえず、挙動は判ったのでDromeについてはこの辺にしておきます。 それにしても、昨日からかなりの数の3DEngineを試してみているんですが、実際、結構な数のエンジンがあるわりに、日本人ってほとんど使ってない感じですね。 もしくは使ってるけど「つかってまーす」とは言ってないのか。 DirectXやOpenGL、SDLでポツポツ書けるほど、リアルタイムCG技術って簡単じゃなくなってきてるんだけど、やっぱり学校でOpenGLのAPIで適当なところまでしか教えないからこうなるのかなあ…。 まあゲームを作れ、とは言わないけど、世間の技術が上がる速度(上記の例のように2005年なのにもう化石化が進んでる…)に対して、大学・大学院の教育レベルって上がってないよなあ。 全然関係ないけど、 ボスがIEEE VR2007から帰ってきました。 ジオメトリテクスチャの論文がすでに存在していてびびりましたよ。 うかうかしていると、論文に何が書いてあるかも理解できなくなる。