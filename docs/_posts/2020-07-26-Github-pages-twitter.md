---
title: "Github Pages 移植進行中。markdownでのTwitter埋め込み"
date: 2020-07-26
author: aki
---
[2006年の1年分のBlog](https://kaitas.github.io/blog/)をアーカイブした。
まるまる4連休使い切ったが後悔はしていない。
2006年はどうしてこんなに一生懸命ブログを書いていたのだろうか…その時の気持ちを思い出すのは難しい。

- JSPSの海外特別研究員だった → 日報的なものを残すのが使命と考えていた
- 海外在住者のブログがおもしろかった
- アメブロ, mixi 全盛期

たぶんその辺がモチベーションなんだけど、そのあと国の機関に勤めるようになって自由な発言は封じられてしまい、大きなトラウマを背負った。
そこで大学の先生になっていれば、少しは変わっただろうか？
でも「こんな文章を書いて世間に見せるなんて恥ずかしい」という気持ちは常にある。振り返るのも相当にエネルギーが必要だ。

自分が成長しているんだということを言い聞かせる。

さて、markdownによるブログ。

Twitterも埋められるようになった
例えばこんな感じ。

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">@mogmogvr そうですね！
挑戦として、目指すものとして悪くないけど、一方で非常に難しいことであること。
これを常識として理解してもらう必要があるフェーズにあると思います。
私も挑戦する側ですが、何も知らずに騙される人がいたら可哀そう、という視点については同意したいところです。</p><a href=" http://twitter.com/o_ob/status/1287417498216751104"> July 27, 2020 at 01:00AM</a></blockquote>

かつてWordpress上ではTwitter Digestというプラグインをカスタマイズして遺してきた。

Twitterのアーカイブは過去、大きなテーマだったのだけど、最近はTwitter公式の``widget.js``を使う方法がよいと考えている。
（見た目の問題と利用規約的な理由）

なお公式の引用方法だと、結構長いスクリプトになるが、実は ``blockquote`` で ``A`` タグを囲んでtwitter参照URLを書けば良い。
オプションで引用元ツイートを表示しないオプションもある。
具体的にはこんな感じ。

> &lt;blockquote class="twitter-tweet" data-conversation="none"&gt;&lt;a href="https://twitter.com/o_ob/statuses/1267113139851558912"&gt;&lt;/a&gt;&lt;/blockquote&gt;

という感じで``data-conversation="none"``を加えてあげることで引用RTの元ツイートを表示しない。
TwitterからIFTTT経由でTweetを保存するときにこのタグを加えてあげれば、そんなに難しいことではなくなる。

# iPhoneで書く markdown エディタ

なお、このエントリーはiPhoneで書いている。
なんとか書ける、というレベルではあるが
- Working Copy
- GitHub 公式アプリ
- Type

を比較している。
Github操作では Working Copy がなかなか素晴らしい、本家よりいい。
Typeはプレビューがいい。

しかし、できれば両手良指で作文する時間を確保したいと思った。

さて仕事しよう。

