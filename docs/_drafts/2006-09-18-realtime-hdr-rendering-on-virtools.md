---
author: ameblo
title: "\n\t\t\t\tRealtime HDR Rendering on Virtools\t\t"
slug: realtime-hdr-rendering-on-virtools
id: 3017
date: '2006-09-18 21:23:48'
layout: post
categories:
  - '[Re]virtual reality'
---

久々に公式HPを見に行ったら面白いデモがありました。 **Virtools High Dynamic Range Car Demo** [http://www.virtools.com/applications/technology-hdrcar.asp](http://www.virtools.com/applications/technology-hdrcar.asp)

Concept: A Demo Showing High Dynamic Range (HDR) Rendering, Image Based Lighting (IBL), Dual Tone Car Paint and Post-Processing Effects. Showing off Virtools™ 4's high end rendering capabilities, this car demo illustrates some of the latest real-time HDR Rendering techniques using multiple shaders. Some of the HDR Rendering features include floating point texture and render target, tone mapping, natural eye adaptation (auto exposure) and glow. This demo also shows Virtools 4's image based lighting shader capabilities, using an environmental texture to compute the car's lighting. コンセプト：高ダイナミックレンジ(HDR)レンダリング、画像ベースライティング(IBL)、車体に対する複数トーンペイント、ポストプロセスエフェクトのデモ。 Virtools 4のハイエンドレンダリング可能性の紹介。このcar demoは最新のリアルタイムHDRレンダリング技術を複数のシェーダーを使って表現している。HDRレンダリング機能は浮動小数点テクスチャとレンダリングターゲット、トーンマッピング、自然な目への適合(自動露光)とグロウを含んでいる。このデモはVirtools 4のIBLシェーダー機能、すなわち環境テクスチャを車のライティングへの演算…も示している。

[![](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo1.jpg)](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo1.jpg) [![](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo2.jpg)](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo2.jpg) [![](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo3.jpg)](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo3.jpg) [![](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo4.jpg)](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo4.jpg) [![](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo5.jpg)](http://akihiko.shirai.as/modules/bwiki/index.php?plugin=ref&page=Virtools%2FHDR&src=HDRdemo5.jpg)

DirectX9, VS_2.0必須とのことです。PS_2.0ではなくてもいいみたいですね(試してません)。 [http://adv3d.jp/](http://adv3d.jp/)

 でやっていたころのリアルタイムGI+HDRレンダリングに近い結果を得られるものが研究室に届く時代がやってきてしましたねえ…。 しかし床との影が気になるよなあ。 HDRレンダリングではハードシャドウは出づらいですし、Virtoolsのレンダリングエンジンは完全なGIでもないでしょうから、うまく代表光からソフトシャドウを投げてあげるような演出はあったほうがよかったも。 あとHDRは.hdr形式をサポートするんだろうか？？ とりあえずソースがないから想像の範囲を出ませんが。 HDRレンダリング自体はさほど珍しいものではなくなりつつありますが、リアルタイムで共通の方式(たとえばHDRIファイルですら、.hdr、OpenEXRなどさまざまある…)がないので、Virtoolsでサポートするとなると、いろいろ使いでがでてきますね。 ちなみにVirtoolsはダッソーに買われた事で、こういう車産業寄りのデモが増えていいことですね。わかりやすいし。 といいつつHDRレンダリングを分かりやすくというのであれば、車のマテリアルはオペークホワイトとかがいいよなあ。 欲を言えば、車だけじゃなくて、石像とかで比較してみたくもあるのですが。 まあ買ってからやってくれ、ということですかねえ。

細かいことは19日の「Virtools Day」で聞いてみよう…うちの研究所で開催するんだし。 [http://www.clarte.asso.fr/](http://www.clarte.asso.fr/) なお、デモのFSAAはフルスクリーンアンチエイリアシングですね。ONにしたほうが良いでしょう。印象がぜんぜん違うはず。あとAutoExposureは最初はOFFで遊んで見ましょう。 人間の目の露出にあわせているだけではHDRレンダリングの面白さはわかりませんし。 ここに追加の写真と解説をおいておきます。 [http://akihiko.shirai.as/modules/bwiki/index.php?Virtools%2FHDR](http://akihiko.shirai.as/modules/bwiki/index.php?Virtools%2FHDR)