---
author: ameblo
title: "\n\t\t\t\tPapers/Performance Capture\t\t"
slug: papersperformance-capture
id: 3325
date: '2007-08-08 23:56:55'
layout: post
categories:
  - SIGGRAPH
---

NPARがはやくおわり、途中から聴講。 「Practical Motion Capture in Everysay Surroundings」 技術の核のところが聞けなかったがGPS使用？ 関節角度ベースの技術。 自転車、筋トレマシーン、卓球、車の運転、スキーなどの動作をスキンアニメーションで再現していた。 評価として Viconの再構成とも比較している。 角速度の算出に利点がある。 Inertial+ultrasonicはドリフトが少ない。 Q&Aより 18センサー使用。 ビデオをみていると本当に、磁気センサらしきものしかついてない。 あとは慣性力センサーか。 Q：人間以外で試したことがあるか？ A：No Q:rootポジションは？ A:とってません （たくさんセンサがあるからとらなくてもいいんだと思われる） 「Prakash: Lighting-Aware Motion Capture Using Photosensing Markers and Multiplexed Illuminations」 Ramesh Raskarが講演。ほか共著者たくさん。 見えないマーカータグを使って屋外で500Hzのモーションキャプチャ。 高速な赤外線マルチアレイを使ったプロジェクタとフォトセンサによるタグで構成。 位置も取れるが方向も取れる。 布にマトリクス状におけば３次元布シミュレーションもオーバーレイできる。 プロジェクタが左右に走査線を走らせればいいわけだが60Hzは遅すぎる。 binary gray codesを変調したIR光源でてらせば500Hzで撮れる。 この変調光源を複数並べればいい。 なるほどねえ。 都合により途中退席。。