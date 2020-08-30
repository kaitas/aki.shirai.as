---
author: ameblo
title: "\n\t\t\t\tWiinority Report Interface\t\t"
slug: wiinority-report-interface
id: 3430
date: '2007-11-14 08:02:19'
layout: post
categories:
  - '[発刊!!]WiiRemote'
---

ファビアンに教えてもらったVR Geek Blogからのネタなのですが [http://cb.nowan.net/blog/2007/11/13/multitouch-with-the-wiimote/](http://cb.nowan.net/blog/2007/11/13/multitouch-with-the-wiimote/)

CMUのJohnny Leeさんが開発したWiiRemoteをつかったマイノリティ・リポート的UI。 マイノリティであることは間違いないので「Wiinority Report Interface」と名 づけることにします(笑)。 [http://www.youtube.com/watch?v=0awjPUkBXOU](http://www.youtube.com/watch?v=0awjPUkBXOU)

うーん、まあIR-LEDアレイを使って…ってのは一般的よくやる構成ですけど、WiiRemoteのはカメラじゃないですからね（Leeさんはカメラといっているように聞こえるけど）。最終的に反射板使ってるんならLEDでいいじゃん、と思いますが。デモの中盤で出てくる手をウネウネ検出するあたりのほうが興味あります。

たぶん本人はこれで何かやりたかったようにも思いますがS/Nというか、制御が難しいので（IRセンサーの特性と同時2点しか検出しない仕様上の制約）最終的にこうなっちゃったような感じがします。 でもパーティクル使って、履歴を残すのはうまい方法だと思います。 これだと値が飛んだときもそこそこ対応できるかもしれない。 (WiiRemoteのIRセンサ値は、2つのグループの重心のようなものを出力しますが、インデックスや強度などは送らないし、インデックスも入れ替わる可能性がある) デモのズームとかの例は、ほとんど定番と化してますが、下手にかっこいい映像でごまかさずに、メッシュにしたのは好感もてます。せっかくならiTouch でできるようなことだけじゃなくて、握ったりつぶしたりもできればよかったのに！ それにしてもトランプってこんな使い方もあるかあ。 自分ならPatafix(3Mの貼って剥がせるゴム)を使うけどね！ まあでもすごいPageviewですね。 私のところにもいろんなところから「みたー？」ってメールが来ますし。 SIGGRAPH E-Techにこのネタで通ったりするんでしょうか？ だったら「もっとすごいもん」を投稿したくなってくるんですけど！ とりあえず最終講義の準備に戻ります。

追記。

その後、CMUのJohnny Chang Leeさんについて調べてみました。 [http://www.cs.cmu.edu/~johnny/academic/](http://www.cs.cmu.edu/~johnny/academic/) 博士の学生みたいですね。2008年PhD取得予定。 MERLで2002-2006までプロジェクタ関係でインターンをしていたようです。関連特許も沢山。

最新の研究もすごく面白い。 [http://www.youtube.com/watch?v=nhSR_6-Y5Kg](http://www.youtube.com/watch?v=nhSR_6-Y5Kg)

赤外線同軸光学系をちょうど2003-2004年ごろやっていた身としても、評価できますね。

とりあえずWiinority型は自分で試してみようかな？