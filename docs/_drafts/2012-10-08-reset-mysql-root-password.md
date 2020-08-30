---
author: aki
title: "\n\t\t\t\tmysqlのrootパスワードを忘れたら\t\t"
slug: reset-mysql-root-password
id: 4369
date: '2012-10-08 22:42:21'
layout: post
categories:
  - network
  - Wordpress
tags:
  - Server
  - wordpress
---

mysqlのパスワードって必要な人には必要なんだろうけど，必要ない人にとっては本当に忘れそう…． しかもphpのソースコードにも書いてあったりするから，迂闊なマスターパスワードを設定したら，逆にセキュリティホールになってしまいそうだし． で，root@localhostのパスワードを忘れました．すみません． たぶん，centos6のyumでインストールした後，セットアップスクリプトが走るのですが，そこで設定したパスワードをすっかり忘れたようです． メモは取る癖をつけているのに何も残ってないので，恐らく寝落ちしたのでしょう． どこまでセットアップが終わっているのかもわからないので，アンインストールしてしまえばいいのかもしれないのですが， 「もし生きているサービスを消してしまったら…」と思うとしのびないので，rootのパスワードだけ初期化してみます． 参考： [http://dev.mysql.com/doc/refman/4.1/ja/resetting-permissions.html](http://dev.mysql.com/doc/refman/4.1/ja/resetting-permissions.html "http://dev.mysql.com/doc/refman/4.1/ja/resetting-permissions.html") 使っている環境ではmysql-server-5.1.61-4でした．

<pre> /usr/libexec/mysqld --skip-grant-tables</pre>

ではうまく行かなかったので，

<pre>mysql -u root mysql
mysql> UPDATE user SET Password=PASSWORD('passwdh0geh0ge') WHERE User='root';
mysql> FLUSH PRIVILEGES;</pre>

という感じに，mysqlの管理テーブルを直接更新して，

<pre>/etc/rc.d/init.d/mysqld restart</pre>

するだけで片付きました． ちなみにもともとやりたかったのは，wordpress用のDBを作りたかったので，ついでにやってしまうべきでした． 参考：[http://www.adminweb.jp/wordpress/install/index1.html](http://www.adminweb.jp/wordpress/install/index1.html "http://www.adminweb.jp/wordpress/install/index1.html")

<pre>create database wpdb;
grant all on wordpressdb.* to 'wpadmin'@'localhost' identified by 'password';</pre>

これでwpdbというデータベースがwpadminというユーザ，パスワードはpasswordで作成されました．インストール時にこれを設定すれば良いわけです． 以上一件落着！