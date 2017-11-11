# ブラウザだけでGitHub Pages
## はじめに
GitHub Pagesとは、GitHubにおける静的ウェブサイトの公開機能である。
任意の方法で静的ウェブサイトを構築したときの公開方法は
[ここ](https://qiita.com/kuronat/items/99d7a2c9b566141636f2)
に書いた。
ところで、GitHubの機能をよくみてみると、GitHub Pagesの作成や更新は、ブラウザ上だけで完結させることができる。

## 大まかな流れ

* リポジトリを作成
* 好きなテーマを設定
* `index.md`を作成
* `_posts/YYYY-MM-DD-your-title.md`を作成
* しばし待つ
* 完成

## Jekyll
Jekyllとは静的サイトジェネレータである。同様のツールにHexo, Hugo, Pelicanなどがある。

JekyllはGitHub Pagesでは特別扱いされている。リポジトリにコミットするたび、GitHub側でJekyllのビルドが行われる。GitHub側がビルドをしてくれるので、手元でビルドしてpushする必要がない。おかげで、ブラウザを使った操作だけで静的サイトを構築することができる。

テーマを変更するのも簡単で、リポジトリの[Settings]から設定が行える。[Change Theme]の操作は `_config.yml` 設定ファイルの編集&コミットと同様である。

## ファイルの編集
ブラウザから、GitHub上のリポジトリのファイルを編集することができる。

* 🖊アイコンで編集
* 🗑アイコンで削除

この編集は、リポジトリに対するコミットとなる。

* Jekyllビルドに対応するようなMarkdownを作成しコミット
* コミットされたことでJekyllのビルドが実行される

つまり、ブラウザ上の操作だけで静的サイトの作成・更新が行える。

## 記事の追加
Jekyllビルドに対応するようなMarkdownを作成するには、以下の命名ルールがある。

* `index.md`
* `_posts/YYYY-MM-DD-your-title.md`


たとえば、

* [_posts/2011-12-31-new-years-eve-is-awesome.md](https://github.com/kuronat/play-jekyll/blob/master/_posts/2011-12-31-new-years-eve-is-awesome.md)

に対応するURLは

* https://kuronat.github.io/play-jekyll/2011/12/31/new-years-eve-is-awesome

となる。詳細は[ここ](http://jekyllrb-ja.github.io/docs/permalinks/)を見る。
