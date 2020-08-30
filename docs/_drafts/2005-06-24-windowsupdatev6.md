---
author: ameblo
title: "\n\t\t\t\tWindowsUpdateV6\t\t"
slug: windowsupdatev6
id: 2226
date: '2005-06-24 05:03:18'
layout: post
categories:
  - network
tags:
  - Server
---

Windows2003server でSP1を当ててからというもの、 「0x80072efd」というエラーが出てWindowsUpdate出来なくなる。 この辺にそれらしき情報はあるんだが、ちょっと見当違い。 [http://support.microsoft.com/?scid=kb;ja;875273](http://support.microsoft.com/?scid=kb;ja;875273)なんとなく原因は分かってる。 プロクシは使っていないので、ネットワークのルーターが正しく振舞っているだけだ。 syslogとWindowsUpdate.log(V6から"Windows"と"Update.log"の間のスペースがなくなった)とにらめっこしていたら、「https://update.microsoft.com/v6/ClientWebService/client.asmx」というURLが取れなくてProxyを試しているようだ。 てゆーか、だったらそういうエラーを出してくれよと、お粗末具合を指摘したくなる。 しかもこのupdate.microsoft.comというのがこまったもんで、apt-getのようにクライアントが80番にアクセスできればいい、とか信頼済みサイトになってればいい、というわけではなくて、なんと443番のポートを開けなければならないという仕様のようだ。 443番というのHTTPSで暗号化通信だけど、まさか向こう側からの通信まであけないといけないとは。当然ながら普通のルータは「閉じる」という設定になっている。しかも当のサイトのIPアドレスは年がら年中変わるので、現在は「222,207.46.198.93」であるが、他のWin2kサーバなどのためにも以下のようなIPに443番からのアクセスを許すよう設定している。 「64.4.20.220,207.46.244.222,207.46.198.93」 当然、というか、いつものこととなりつつあるが、こういう情報はMicrosoftのサポートには書いてない。 WindowsUpdateにかかわるサポートは無料で受けられるらしいが…めんどくさいのでせいぜいオンラインサポートでフィードバックするぐらいか。 高いソフトなのにひどい話だなあ。