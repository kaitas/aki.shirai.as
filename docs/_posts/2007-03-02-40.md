---
author: ameblo
title: "\n\t\t\t\tLDAP on Windows+ThunderBird\t\t"
slug: ldap-on-windowsthunderbird
id: 3171
date: '2007-03-02 03:05:08'
layout: post
categories:
  - network
tags:
  - Lucas
---

はあどでぃすくがひどいことになってるのでスキャンディスク中。 …なので、ちょっとわき道にそれた技術調査とかいろいろやってる。 ※しかも今回完結してません。 LDAPって大規模環境(たとえば大学のコンピュータ演習室とか)でログオン一括管理するためのデータベースだと思ってた。 (LはLoginのなんとか、とか) けど、実際には「Lightweight Directory Access Protocol」の略で、まあ簡単に言えば階層化された軽いアクセス(データベース)プロトコル、という話。DNSとかにも似てる。 プロトコルはともかく、これがなぜメールソフトに実装されてるのか長いこと謎だった。Notes使ってたときの「社内のどこの部署にいるなんとかさん」を探すのに使えるのね。でも個人で使うならNotesほど遅くないだろうし、ノートPCやLinux、Windows、リモートデスクトップサーバと散りに散ったメールアドレスをうまく管理できるんじゃないか、と思った。 てゆーかそういう需要ってないんですか皆さん！！ みんなGmailがあればそれでいいってわけ？ ちなみにOutlook ExpressでもActive Directoryとかと連携してLDAPもどきが実装されてる。Windowsｓサーバーにもそれらしきサービスはある(がもちろん使わない)。まずActiveDirectoryがらみで何かいいことがあったためしがないので。 そんなわけで、OpenLDAPをLinuxに入れてみる。なんだかわけ判らん、そもそも自分で使ったことないプロトコルをサーバーにインストールするのはテストもできないのでつらい。 というわけでとりあえずOpenLDAP for Windowsを使って試してみようと思った。 OpenLDAP for Win32 [http://lucas.bergmans.us/hacks/openldap/](http://lucas.bergmans.us/hacks/openldap/) ドキュメントはほとんどついてない、OpenLDAP本家を見ろという。 QuickStartがあるけど、OpenLDAP fow Win32の初期パスワードがわからん…。 [http://www.openldap.org/doc/admin23/quickstart.html](http://www.openldap.org/doc/admin23/quickstart.html) この記事は比較的読めた。 [http://www.atmarkit.co.jp/flinux/rensai/linuxtips/910ldap2mail.html](http://www.atmarkit.co.jp/flinux/rensai/linuxtips/910ldap2mail.html) ちなみにLDIFファイルはThunderBirdからエクスポートできますね。 ちなみにJavaでLDAPdなるサーバとか、ブラウザもあるらしい。 [http://muimi.com/j/ldap/](http://muimi.com/j/ldap/) Appletもある。 [http://www-unix.mcs.anl.gov/~gawor/ldap/](http://www-unix.mcs.anl.gov/~gawor/ldap/) slapdのパスワードがわからん。 slapd.confでdcに仮のドメイン名を設定して、 rootpw secret としているんだけど、ldifファイルの読み込みで ldapadd -x -D "cn=Manager,dc=testdomain,dc=as" -W -f test.ldif ここでパスワードを聞かれてしまう。もちろん「secret」ではない。 MD5とかつかったらいいのかしらん。 おしえてえらいひと！