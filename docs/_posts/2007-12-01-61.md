---
author: ameblo
title: "\n\t\t\t\tWiiYourself!0.96b for Multi-WiiRemote connection\t\t"
slug: wiiyourself0-96b-for-multi-wiiremote-connection
id: 3449
date: '2007-12-01 02:46:40'
layout: post
categories:
  - '[発刊!!]WiiRemote'
---

WiiYourself!0.96bは赤外線LED4点検出やスピーカーからのWAV再生などに対応していて機能面ではかなり充実したAPIなのだけど、残念なのはマルチWiiRemote接続に対応していないこと。対応してないはずないんだけど、通信スレッドに個々のWiiRemoteのIDやデバイスパスが渡せないので、APIのコアに手を入れないと駄目かな、というところまではたどり着いていた。

簡単に表現すると cWiiYourself.Connect(0); cWiiYourself.Connect(1); とすると、1としか通信してくれない。

単純にEXEを重複起動してみると、ちゃんと2つのWiiRemoteと通信するので、MUTEXなりスレッドセーフなり、GUIDなりハンドル渡しなりにすれば動くのでは、と思う。

ライセンス的にはかなりオープンだけど「クレジット表記、競合的なライブラリを作らないこと」とあるので作者に連絡してみたけどいまのところ連絡なし。

WiimみたいにHID管理クラスと<vector>をつかって各WiiRemoteのハンドルを管理したほうがいいように思うんだけどな。

4点検出のデモはソース、EXEつきでここにおいておきます。 [http://akihiko.shirai.as/modules/mydownloads/viewcat.php?cid=6](http://akihiko.shirai.as/modules/mydownloads/viewcat.php?cid=6)

とりあえず、VirtoolsBBへのコード移植を急ごうっと。

ちなみに7日に開催される私のFarewell party (Pot de depart)が内覧会になったっぽい。 さらに次の日8日に開催されるテクノポールのクリスマス会が本番。

週末カウントしてもあと4日。 正味あと2日。

GillとAlexisのエンジンがかかってきたから、ミラクルは起きると思うよ！

Je desire cette animation va marche bien a l'Arbre de Noël de la Technopole!