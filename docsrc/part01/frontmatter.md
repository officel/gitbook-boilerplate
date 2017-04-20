---
description: This is desc.
keywords: gitbook, git, markdown
test: test now.
---

# Front Matter

* ファイルの先頭でハイフン3つの行で挟む
* YAMLとして扱われる
* YAMLとしてNGだとserveが落ちる（buildが通らない）
* descriptionを書いておくと、htmlファイル中のmetaとして扱われる（ソース参照）
  * 同種のmetaのkeywordsは反応しない
* -{{ page.test }}- variablesとしても使用可能（ページ内に限る）
  * これについては本家サイトの説明不足なような気がする
  * 参考用にbook.json中のvariables -{{ book.test1 }}-

* SUMMARY.mdで使用すると目次中のヘッダーとして文字列のまま出力されてしまう
  * descriptionも書くことができない
  * SUMMARY.mdはページ内にインクルードされるので必要ないのかもしれない
