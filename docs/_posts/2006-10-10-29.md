---
author: ameblo
title: "\n\t\t\t\tVista on VMWare\t\t"
slug: vista-on-vmware
id: 3050
date: '2006-10-10 03:09:09'
layout: post
categories:
  - network
---

Windows Vista RC1をVMWare Workstation/Player環境で試してみる。 先日、デスクトップマシンに入れたのだけど、都合で消してしまったので。 ポイントは2点。 .vmxファイルをテキストエディタで開いて以下を追加。 svga.maxWidth = "640" svga.maxHeight = "480" ethernet0.virtualDev = "vmxnet" その後、VMWareToolsをインストール。 ネットワークカードが見つからないのでUSBメモリキーが使えたのはラッキー。 以下参考 [http://pubs.vmware.com/guestnotes/wwhelp/wwhimpl/common/html/wwhelp.htm?context=guestos&file=guestos_winvista.html](http://pubs.vmware.com/guestnotes/wwhelp/wwhimpl/common/html/wwhelp.htm?context=guestos&file=guestos_winvista.html) [http://mkosaki.blog46.fc2.com/blog-entry-32.html](http://mkosaki.blog46.fc2.com/blog-entry-32.html) [http://d.hatena.ne.jp/stealthinu/20060614/p1](http://d.hatena.ne.jp/stealthinu/20060614/p1) VMWare上で8色→フルカラーになった瞬間はうれしかったよ。 ついVistaに転びそうになった。 でも解像度640x480から変えられない。だめじゃん。。。 VMWareToolsを最新のものからqemuをつかって引っ張り出すという方法があるらしいが…やくざだなあ。 とりあえず今日はここまで。