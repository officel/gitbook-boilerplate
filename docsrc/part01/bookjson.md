# book.json

* see https://toolchain.gitbook.com/config.html
* [JSONLint](http://jsonlint.com/)に従っているようで気が利かない
  * "key": "value" のようにダブルクォーテーションで囲む必要がある
  * 文字列の場合は必須。必然的にキーは囲っていないとエラーになる
  * 本家サイトのサンプルは囲っていないものがあり、十分にテストされていないものである可能性がある
  * true/false, 123などの数値は囲まなくてもエラーにならない
  * 配列内の最後のカンマは許可されない（余分なカンマはエラーになる）
* i18nというかマルチ言語対応は試していない
* Structureも変更する必要を感じていないので試していない
* 前述の設定のマニュアルには書かれていないが、テンプレートで使用できる変数を埋めることができる
  * {{ book.test1 }} はbook.json中の変数

## book.json now

このリポジトリのbook.jsonの中身

<pre>
{% include "git+https://github.com/officel/gitbook-boilerplate.git/book.json"  %}
</pre>


@todo

* pdfオプションについてテスト
