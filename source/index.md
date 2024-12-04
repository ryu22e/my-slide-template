# 自作のスライドテンプレートの話

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>
<small>This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.</small>

## 自己紹介

* 筒井 隆次
* さくらインターネット株式会社 クラウド事業部 クラウドサービス部 サービス開発 バックエンド所属
* Python歴は13年くらい（主にDjango）
* 趣味: 映画鑑賞、格闘技経験、立ち飲み屋巡り

## 今日話すこと

* 私が今まで使ってきたスライド共有サービスの変遷
* 現在のスタイル（自作のスライドテンプレートの話）

## 私が今まで使ってきたスライド共有サービスの変遷

発表をするようになった当初は、MacのKeynoteでスライドを作って発表後にPDFをスライド共有サービスにアップロードしていた。

### 1. SlideShare

* URL: <https://www.slideshare.net/>
* 2013年ごろから使っていた
* 昔は使いやすかったが、ある時からスライドの最後のページを表示すると、次のスライドに遷移するようになってしまった

### ちなみに当時のスライドはこちら

<https://www.slideshare.net/slideshow/pycon-17250047/17250047>

### 2. Speaker Deck

* URL: <https://speakerdeck.com/>
* 2018年ごろから使っていた
* SlideShareと似たようなサービス
* 日本語のPDFをアップロードすると、アウトラインが文字化けする問題があった
* 回避策はあったものの、毎回これをやるのは面倒だった

## 現在のスタイル

* 結局、外部のスライド共有サービスは仕様が変わることもあるし、どうなるか分からない
* そこで、自前のドメイン`ryu22e.dev`を取ってHTMLで配信することにした

### どのホスティングサービスを使うか

* 今のところ、GitHub Pagesでホスティングしている
* GitHub Actionsで自動デプロイできるので便利
* GitHub Pagesが使えなくなったら別のホスティングサービスに切り替えるつもり

### 自作のスライドテンプレートを作った

* 何度も同じようなスライドを作るのは面倒
* そこで、自作のスライドテンプレートを作った
* URL: <https://github.com/ryu22e/cookiecutter-sphinx-revealjs>
* このスライドも上記のテンプレートを使って作成した

### reveal.jsとは

* URL: <https://revealjs.com/>
* HTMLでスライドを作るためのフレームワーク

### Sphinxとは

* URL: <https://www.sphinx-doc.org/>
* [reStructuredText](https://www.sphinx-doc.org/ja/master/usage/restructuredtext/basics.html#rst-primer)または[MyST Markdown](https://www.sphinx-doc.org/ja/master/usage/markdown.html#markdown)で書いたドキュメントを色んな形式に変換するツール
* 変換できる形式の例: HTML、PDF、ePubなど
* Pythonプログラマーにはおなじみのツール

### sphinx-revealjsとは

* URL: <https://sphinx-revealjs.readthedocs.io/>
* Sphinxでreveal.jsを使ったスライドを作るための拡張
* Sphinxの記法を使いつつ、reveal.jsの機能を使うことができる

### cookiecutterとは

* URL: <https://cookiecutter.readthedocs.io/>
* プロジェクトテンプレートからプロジェクトを作成するツール
* Python製だが、他の言語でも使える

### （時間があれば）デモ
