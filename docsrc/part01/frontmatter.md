---
description: This is desc.
keywords: gitbook, git, markdown
test: test now.
---

# Front Matter

* ファイルの先頭でハイフン３つの行で挟む
* YAMLとして扱われる
* YAMLとしてNGだとserveが落ちる（buildが通らない)
* description を書いておくと、htmlファイル中のmetaとして扱われる（ソース参照）
* それ以外の項目は今のところ使い道がない?
  * 同種のmetaのkeywordsは反応しない
  * -{{ test }}- variablesとしても使えない
  * 参考用にbook.json中のvariables -{{ book.test1 }}-

