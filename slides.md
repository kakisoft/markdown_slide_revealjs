### マークダウンでスライドを作ろう！
### （reveal.js 編）
---
こんな感じのスライドが作れます。
---
[reveal.js](https://github.com/hakimel/reveal.js/) というライブラリを使っています。
---
内容は、マークダウンで記述できます。
（今回は、[reveal-ck](http://jedcn.github.io/reveal-ck/) というライブラリを使っています。）
---
作ったスライドは、Github pagesにて公開する事が可能です。
---
作り方
---
reveal-ck をインストール。（要 ruby 2.4.4以上）
※2020年1月時点
```
sudo gem install reveal-ck
```
---
スライド作成用のディレクトリを作成し、「slides.md」というファイルを作成します。

```
（例）
mkdir markdown_slide_revealjs
cd markdown_slide_revealjs
touch slides.md
```
---
slides.md に、スライドの内容を記述します。

（以下、作成例）
```
### マークダウンでスライドを作ろう！
### （reveal.js 編）
 ---
こんな感じのスライドが作れます。
 ---
[reveal.js](https://github.com/hakimel/reveal.js/) というライブラリを使っています。
 ---
内容は、マークダウンで記述できます。
（今回は、[reveal-ck](http://jedcn.github.io/reveal-ck/) というライブラリを使っています。）
 ---
作ったスライドは、Github pagesにて公開する事が可能です。
 ---
作り方
 ---
（以下略）
```
「---」が改ページとなります。
---
スライドの実態を作成するコマンドを実行します。
```
reveal-ck generate
```
「slides/」が生成されます。
---
その後、スライドを表示するコマンドを実行。
```
reveal-ck serve
```
---
こんな感じのスライドが作れます。
---
slides.md を編集すると、  
自動で変更内容が反映されます。
（ホットリロード）
---
他、色々上手くいってない部分があるけど、  
続きは明日書く。
---
具体的には、
「config.yml」というファイルにコンフィグを記載する事ができるんだけど、そのファイル作って generate を実行するとエラーが出る。
```
error: undefined method `new_ostruct_member' for #<RevealCK::Config:0x00007fda1704bf98>
```
調査は後日。
---
あと、自分がやってる Github pagesでの公開方法が、ちょっと不恰好。  

きっちりやっといた方がいい？  でも、別に今の方法でもいいんじゃね？という考えもよぎる。  

自分がこのライブラリでやりたかった事って、
「クオリティ的には30点でも、瞬足でそれなりの形にする」という事だし。
---
To be continued
---










