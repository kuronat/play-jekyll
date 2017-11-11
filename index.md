# ブラウザだけでGitHub Pages
## はじめに
GitHub Pagesとは、GitHubにおける静的ウェブサイトの公開機能である。
任意の方法で静的ウェブサイトを構築したときの公開方法は
[ここ](https://qiita.com/kuronat/items/99d7a2c9b566141636f2)
に書いた。
ところで、GitHub Pagesは、あまり言及されることはないが、
ブラウザからブログを更新することができる（と思う）。

## ファイルを編集
(GitHub Pagesに限らないことであるが)Markdownファイルは、
🖊マークのアイコンを押すと、ブラウザ上で編集することができる。

この編集は、リポジトリに対するコミットとなる。

## Jekyllで公開
Jekyllとは静的サイトジェネレータのひとつである。似たツールにHexo, Hugo, Pelicanなどがある。
GitHubではJekyllは特別扱いされている。

Jekyllであれば、ブラウザを使った操作だけでブログを立ち上げることができる。具体的には、適当な空のリポジトリを作ってから、
[Settings]を開く。テーマの変更は [repository settings](https://github.com/kuronat/play-jekyll/settings)から行える。
この操作によって、 `_config.yml` 設定ファイルが書き換わる。

リポジトリにコミットするたびに、GitHub側でJekyllのビルドが行われる。
つまり、ブラウザ上の操作だけでブログの更新が行えるということである。

## ディレクトリ構造

* `./index.md` 
* `_posts/xxx.md`
