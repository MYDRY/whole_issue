# whole_issue

主に開発について MyDry 全体に関わることをまとめるリポジトリ

# About branches

### 命名則
さすがに `dev/*` と `develop/*` が混在するのはいただけないので・・・

ぼく個人としての分け方はこんな感じでした。

***
* `master`:
  メインブランチ。常にリリース可能な状態であることが望ましい。
  なので基本的に他のブランチからの pull request を受けるだけ。

* `develop/*`:
  `master` から生やす*統合ブランチ* 。普段の開発は主に`develop` から生やした 
  `feature/*` ブランチを使う。
  基本消さない。  (つまり `master` と `develop` は常に生きてる状態)

* `feature/*`:
  `develop` から生やす*トピックブランチ* 。
  今までの使い方でいくと、`develop` を更に細切れにしたイメージ。
  `develop/*` に統合される。

* `fix/*` or `hotfix/*`:
  バグ修正用ブランチ。緊急時に`master` から切られるのが `hotfix`。
  俺はこれと別に `develop/*` から切る `fix/*` みたいな使い分けをしてる。
  特に意味があるわけじゃないけど。

* `release/*`:
  リリース準備用のブランチ。\* にはバージョン名を書くのがいいかもしれない
***

**\* の部分にはそのブランチの作業内容がわかるような名前をつける**
ハイフン区切りが気に入ってるんだけどどうでしょうか。

例）`develop/add-image-preview`

参考文献：
[ブランチの運用](https://backlog.com/ja/git-tutorial/stepup/stepup1_2.html)
[トピックブランチと統合ブランチでの運用例](https://backlog.com/ja/git-tutorial/stepup/stepup1_5.html)

### その他
**ブランチは原則、生えてきたところに統合する**
pull request で間違いやすいから注意してね


# About Issues

# About Scrum

# About TDD
