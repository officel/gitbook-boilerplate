# Markdown Samples

* see [Markdown ・ GitBook Toolchain Documentation](https://toolchain.gitbook.com/syntax/markdown.html)
* see [Mastering Markdown ・ GitHub Guides](https://guides.github.com/features/mastering-markdown/)
* see [Basic writing and formatting syntax - User Documentation](https://help.github.com/articles/basic-writing-and-formatting-syntax/)

## TL;DR

* GitBookのマークダウン記法はGFMに近い
* タスクリスト、絵文字は使えない
* それ以外はほぼ問題ない

## Toc

* [Headers](#headers)
* [Emphasis](#emphasis)
* [Lists](#lists)
* [Images](#images)
* [Links](#links)
* [Blockquotes](#blockquotes)
* [Inline code](#inline-code)
* [Syntax highlighting](#syntax-highlighting)
* [Tables](#tables)
* [Task Lists](#task-lists)
* [Emoji](#emoji)



## Headers

Setext-style

```
header1
======
header2 {#setext-h2}
------
```
ex

header1
======
header2 {#setext-h2}
------

link to [Setxt-style header2](#setext-h2)

---

Atx-style

```
# header1 {#atx-h1}
## header2
### header3
#### header4
##### header5
###### header6
```

ex

# header1 {#atx-h1}
## header2
### header3
#### header4
##### header5
###### header6

link to [Atx-style header1](#atx-h1)



## Emphasis

```
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

~~This text will be crossed out.~~
```

ex

*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

~~This text will be crossed out.~~

つまり*イタリック*、**ボールド**、_その__入れ子__も_できて、~~打消し線~~も引ける。
また、*イタリック*__ボールド__のように記号を変えればくっつけて書ける。



## Lists

### Unordered

```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
    - Item 3a
```

* Item 1
* Item 2
  * Item 2a
  * Item 2b
    - Item 3a

### Ordered

```
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```

1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

### DL

```
<dl>
<dt>りんご</dt>
<dd>赤いくだもの</dd>
</dl>
```

<dl>
<dt>りんご</dt>
<dd>赤いくだもの</dd>
</dl>

DLはそのままマークアップする。



## Images

```
![google Logo](https://www.google.co.jp/images/branding/googlelogo/2x/googlelogo_color_120x44dp.png)

![google Logo](https://www.google.co.jp/images/branding/googlelogo/2x/googlelogo_color_120x44dp.png "Search")
```

![google Logo](https://www.google.co.jp/images/branding/googlelogo/2x/googlelogo_color_120x44dp.png)

![google Logo](https://www.google.co.jp/images/branding/googlelogo/2x/googlelogo_color_120x44dp.png "Search")

GitBookはsvgだったのでやむなくgoogleロゴに。画像の表示は`![Alt Text](url "Title Text")`ということ。



## Links

```
http://gitbook.com 

[GitBook](http://gitbook.com)

[GitBook](http://gitbook.com "GitBook ・ Documentation made easy")
```

http://gitbook.com 

[GitBook](http://gitbook.com)

[GitBook](http://gitbook.com "GitBook ・ Documentation made easy") 画像と同じようにタイトル付が使える



## Blockquotes

```
As Kanye West said:

> We're living the future so
> the present is our past.
```

As Kanye West said:

> We're living the future so
> the present is our past.



## Inline code

```
変換するには`gitbook build`と打つ
```

変換するには`gitbook build`と打つ



## Syntax highlighting

    ```javascript
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    ```

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

単にインデントするだけでもコードのように表示できる



## Tables

see [Organizing information with tables - User Documentation](https://help.github.com/articles/organizing-information-with-tables/)

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

---

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

***

| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |

* * *

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

- - -

| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |




## Task Lists

GFMの機能なのでGitBookでは使用できないようだ。

```
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
<!-- textlint-disable --> 
- [ ] this is an incomplete item
<!-- textlint-enable --> 



## Emoji

:simple_smile:

絵文字も使用不可（ドキュメントには不要か）

