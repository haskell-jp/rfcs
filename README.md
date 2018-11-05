このリポジトリは、コミュニティとしてのHaskell-jpを俯瞰し、また改善するための提案を管理するための場所である。

## ガイドライン

IssueまたはPull requestによって、コミュニティレベルでの提案をすることができる。
使い分けの基準は以下の通りである。

* Issue: 内容が単純で、影響が及ぶ範囲が一つである。「問題だけ」を投稿するならこちらを選ぶべきである、
* Pull request: 複数の構成要素に影響を及ぼす。内容が複雑で、複雑な議論を要する。問題と解決法の双方を提示する場合、rfcsディレクトリ以下にMarkdownファイルを作成し、Pull requestとして送ることを推奨する。

Issueを使う動機は投稿の簡単さのためで、一方Pull Requestを用いる動機はレビュー機能により議論をまとめやすくすることである。

また、このファイル自体への変更もPull requestで受け付ける。

文体は常体の口語体を推奨するが必須ではない。体言止めなどのカジュアルな表現を使っても問題はない。

## コミュニティの目的

Haskell-jpの存在する目的は以下の二つである。

* P: 日本にHaskellを普及させる
* Q: 日本を代表するHaskellのユーザーグループとなる

## 構成要素

この節では、Haskell-jpを構成するサービスなどを記述する。技術的な詳細には触れず、Haskell-jpとの関係と効果に着目する。

目標Pを達成するには、コミュニティから、潜在的なユーザーに向けて__発信__する手段が不可欠となる。また、目標Qを達成するには、ユーザー同士の__対話__の場、そしてコミュニティを維持するための__管理__が必要である。目的を達成するための構成要素の役割を __発信__ 、 __対話__ 、 __管理__ の3つに分類し、各項で考察していく。

一つの要素で全ての役割を果たすことも可能だが、それが最善とは限らないことに注意すべきである。レビューなどは発信と対話を分離する好例で、発信する前に情報の質を高めることができる。

### 人々

_役割: 発信、対話、管理_

自明ではあるがコミュニティの存在にはメンバーが不可欠である。他の構成要素を利用して役割を果たす、最も重要な要素である。

人々が単位時間当たりにこなせる仕事には限りがあるため、同じ役割を持つ要素が多すぎると労力が分散してしまい、届きうる情報が散逸してしまうリスクが生まれる。

メンバーの特殊な場合としてコアメンバーがある。コアメンバーは互いに連携を取り、コミュニティの意思決定や、構成要素の管理を行う。

- 人はかなり集まっているように感じる。他の構成要素とのつながりを強化し、成果に結びつけたい - @fumieval

### [haskell.jp](https://haskell.jp/)

_役割: 発信_

後述する構成要素へ案内するポータルサイト。迷ったらここを見ればよい。

- デザインは悪くないが、機能性を重視するならば全てのリンクがページに収まっていると理想的である - @fumieval

### [Slack](https://haskell-jp.slack.com)

_役割: 対話、管理_

議論のほとんどはこのSlack上で行われている。いくつかの自動投稿チャンネルと、トピック別のチャンネルからなる。

いわゆる無課金のため、Slack本体から古い投稿にはアクセスできなくなってしまうが、[slack-log](https://github.com/haskell-jp/slack-log)というツールにより投稿を保存することで対処する。

randomとquestions、haskell-jp-status、event-announcementsの四つのチャンネルがよく利用されている。

- ブロックやミュートなどの機能はないため、ユーザー間のトラブルに脆弱である - @fumieval

### [Trello](https://trello.com/b/GfAyczPt/haskell-jp)

_役割: 管理_

コミュニティのタスクを管理している。変更がリアルタイムに反映される。リアルタイムに更新が反映される、チェックリストを管理できるなど、優れた機能を持つ。編集権限を持つメンバーは一部だが、アカウントさえ持っていれば誰でもコメントを追加できる。内容(≒未消化のタスク)は充実しており、それなりに更新もされている。

- コアメンバーがタスクを共有する場所としてうまく機能していると感じる - @fumieval

### [Twitter](https://twitter.com/haskell_jp)

_役割: 発信_

Twitterアカウントが存在するが、フォロワー数も発言数も少なく、火力不足が否めない。

- Tipsを投稿したり、Haskellに関するツイートを積極的にRTするなどの働きかけにより、より効果的な媒体になると期待している - @fumieval

### [GitHub](https://github.com/haskell-jp)

_役割: 管理、対話_

Webサイト、ロゴ、教材、関連ツールを管理する場所として利用する。比較的議論も活発である。

- この調子でHaskell-jpに属するプロジェクトを増やせば、さらなるアピールになりそうだ - @fumieval

### [ブログ](https://haskell.jp/blog/)

_役割: 発信_

[リポジトリ](https://github.com/haskell-jp/blog)を通して記事を投稿できる。もちろん誰でも閲覧でき、コミュニティの主要な情報発信源であると言える。

- どれだけの人に届いているかを表す指標として__はてなブックマーク__の数が考えられるが、その値はあまり[芳しくない](
http://b.hatena.ne.jp/entrylist?url=https%3A%2F%2Fhaskell.jp%2Fblog%2F)。隙間産業的な内容の多い私の[個人ブログ](http://b.hatena.ne.jp/entrylist?url=http%3A%2F%2Ffumieval.hatenablog.com%2F)よりも中央値が低いので、情報がうまく行き届いていない可能性が高い - @fumieval

### [Wiki](https://wiki.haskell.jp/)

_役割: 発信_

Gititを利用したWiki。GitHubアカウントで認証することで編集が可能。

現在[Haskellに関する日本語のリンク集](https://wiki.haskell.jp/Links)と[データ構造列伝](https://wiki.haskell.jp/%E3%83%87%E3%83%BC%E3%82%BF%E6%A7%8B%E9%80%A0%E5%88%97%E4%BC%9D)の二つが充実しているが、他の内容は少ない。編集の頻度は極めて低く(月に1件未満)、閲覧者も少ないと考えられる。

- Gitリポジトリよりも変更と閲覧の楽なWikiは、知識の集積場所として優れたインターフェイスである。より多くの人が使いたくなるような動機付けが必要であると考えられる - @fumieval

### [Reddit](https://www.reddit.com/r/haskell_jp)

_役割: 対話_

外部リンクの共有と議論が可能な場所であり、コメントがリストではなく木構造をなすのが特徴であり特長である。投票システムにより、人気の投稿はよりアクセスしやすくなり、不評な投稿は隠れる。また、外部からアクセスできるのも大きな違いである。

[r/haskell](https://www.reddit.com/r/haskell)と比較すると投票・コメント数共に極めて少なく、特長が活かせていない。

- 使用を取りやめ、Slackに投稿するように勧めたほうがより多くの人が参加でき、また複数のサイトを追う手間も減らせるのはないか - @fumieval
- Slackと比べると馴染みにくい雰囲気なのかもしれない - @fumieval

### [イベント](https://haskell-jp.connpass.com)

_役割: 発信、対話_

主要なのはHaskell-jpが主催する定期ハッカソン、Haskell-jpもくもく会である。参加者は10〜20人ほど。コミュニティに関する議論や作業がここで行われることもある。4.5時間、おのおのが作業し、残りの30分で軽い発表をすることもある。

- もくもく会は適度に新規参入者がおり、コアメンバーと交流する重要な役割を担っている - @fumieval
- イベントがあるからこそ参加するという層も多い。2018年現在、Haskellについて発表する機会は少ないため、より発表に重きをおいた勉強会を増やすことは有益であると考えている - @fumieval
