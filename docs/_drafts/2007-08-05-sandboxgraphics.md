---
author: ameblo
title: "\n\t\t\t\tSandbox:Graphics\t\t"
slug: sandboxgraphics
id: 3317
date: '2007-08-05 08:35:37'
layout: post
categories:
  - SIGGRAPH
---

**Graphics** True Imposters Eric Risser Displacement Mapping、Parallaax Mapping、Relief Mappingなどあるが「True Impostors」という手法を提案。 カメラのViewing Directionを与えて、quad回転角を得る。4つのhight fieldsを得るQuadsをつかう問題。 見えない部分をどうするか、十分に大きくないといけない（長辺が収まるように）。 [提案手法] 立方体の内側の壁をレンダリング、頂点においてカメラからの正規ベクトルを格納 …詳細は論文参照… Per-Pixel Displacement Mappingにつなぐ。 「どこが正面か？」 原点と視線ベクトルを与える、境界面は各軸の1か-1にある。displacementを軸で割る。 「スケール問題」 テクスチャ空間はいつもキューブ ボリュームから最初のインターセクションを探す いくつかのオプション ・リニアサーチ ・ReliefMapping - Binary Search 「結果」 ・640x480 window 180-190 fpsで10リニアサーチ、8バイナリサーチ ・動物のいろんな視点 ・木星をいろんな視点から、アステロイドの詳細とかも。 **Interactive Shader Development** Peter Dahl Ejby Jensen, Nicholas Francis, Bent Dalgaard Larsen, Niels Jorgen Christensen (Technical University of Denmark) デンマークから。 Quartz Composer風味のシェーダーエディタ。Mac上でうごいてる。 ノードのオプティマイゼーションなども考慮されている。 そういえばEzGPUなんてプロジェクトもやったなあ。。。 会場質問 Q：RenderManのアレと何が違うの？ A：最適化が違う Q：RenderMonkeyと何が違うの A：FXファイルが出てきてうれしいが、最適化については取り組まれてない。 次はGame Design2。