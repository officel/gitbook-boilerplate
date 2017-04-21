---
title: test title
description: GitBook Templating
test: see front matter
test1: ["a","b","c","d","e"]
test2: foobarfoobar
---
# Templating

* see [Templating ・ GitBook Toolchain Documentation](https://toolchain.gitbook.com/templating/)

## Samples

### Variables

| code | value |
| ---- | ----- |
| <code><span>{</span>{ test }}</code>       | {{ test }} |
| <code>{<span>{</span> page.test }}</code>  | {{ page.test }} |
| <code>{<span>{</span> book.test1 }}</code> | {{ book.test1 }} |

* 変数の値がない場合は空になる
* pageはFrontMatterで定義されているもの？
* bookはbook.jsonで定義
* テーブルやリストのmarkdown記法内で<code>``</code>を書いても変数展開されてしまう？

  * このページはマークアップでごまかしてある

    * `<code>`で囲みつつ`<span>`で`{`を1つ囲むことでテンプレートとして認識されないようにしている
    * <code>``</code>で囲むとタグがエンティティ化してしまってダメだった

  * そもそも[本家のドキュメントページ](https://toolchain.gitbook.com/syntax/markdown.html#code)すら壊れていた
  * 後述のescape`{% raw %}`もテーブル内では無効のようだ
  * `{{ page.test }}`

`{{ test }}`, `{{ page.test }}`, `{{ book.test1 }}`このように、パラグラフ中では表現できている。

### Filters

```
* {{ test1 | title }}
* {{ page.test1 | join(",") }}
* {{ page.test2 | replace("foo", "bar") | capitalize }}
```

* {{ test1 | title }}（注：この機能がよくわからない）
* {{ page.test1 | join(",") }}
* {{ page.test2 | replace("foo", "bar") | capitalize }}


