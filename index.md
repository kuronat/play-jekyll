## Welcome to GitHub Pages

### 静的ウェブサイトの公開
GitHubにはリポジトリを利用して静的ウェブサイトを公開する機能がある。
たとえばブログは、静的ウェブサイトのひとつである。

任意の方法で静的ウェブサイトを構築したときの公開方法は
https://qiita.com/kuronat/items/99d7a2c9b566141636f2
に書いた。

### Jekyllによる静的ウェブサイトの公開
Jekyllとは静的サイトジェネレータのひとつで、似たツールにHexo, Hugo, Pelicanなどがある。
GitHubではJekyllは特別扱いされており、ブラウザを使った操作だけで

具体的には、適当な空のリポジトリを作ってから、
![image](https://user-images.githubusercontent.com/30833423/32690415-ba4b241e-c739-11e7-96cb-f698f45b1066.png)
を開く。

### Markdownファイルの編集
[editor on GitHub](https://github.com/kuronat/play-jekyll/edit/master/index.md)
を開いてみよう。Markdownファイルの編集およびプレビューがブラウザから可能である。

本リポジトリにコミットするたび(ブラウザから編集するのもコミットの1つである)、GitHub側でJekyllのビルドが行われる。

### Jekyllテーマの適用

テーマの変更は [repository settings](https://github.com/kuronat/play-jekyll/settings)
から行える。この操作によって、 `_config.yml` 設定ファイルが書き換わる。
