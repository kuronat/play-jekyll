# ブラウザだけでGitHub Pages
## 背景
GitHub Pagesとは、GitHubにおける静的ウェブサイトの公開機能である。

任意の方法で静的ウェブサイトを構築したときの公開方法は
[ここ](https://qiita.com/kuronat/items/99d7a2c9b566141636f2)
に書いた。

ところで、GitHub Pagesは、あまり言及されることはないが、
ブラウザからブログを更新することができる（と思う）。

## ブラウザだけでファイルの編集
(GitHub Pagesに限らないことであるが)Markdownファイルは、
<img height=24 src=https://user-images.githubusercontent.com/30833423/32690453-5c5c87c0-c73a-11e7-9b3d-de43ec603e7e.png>
のアイコンを押すと、ブラウザ上で編集することができる。この編集は、リポジトリに対するコミットとなる。

## Jekyllによる静的ウェブサイトの公開
Jekyllとは静的サイトジェネレータのひとつである。似たツールにHexo, Hugo, Pelicanなどがある。
GitHubではJekyllは特別扱いされている。Jekyllであれば、ブラウザを使った操作だけでブログを立ち上げることができる。

具体的には、適当な空のリポジトリを作ってから、
<img src=https://user-images.githubusercontent.com/30833423/32690415-ba4b241e-c739-11e7-96cb-f698f45b1066.png height=24>
を開く。

テーマの変更は [repository settings](https://github.com/kuronat/play-jekyll/settings)
から行える。この操作によって、 `_config.yml` 設定ファイルが書き換わる。

リポジトリにコミットするたびに、GitHub側でJekyllのビルドが行われる。
