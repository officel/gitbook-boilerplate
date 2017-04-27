# Plugins

* see [Plugins ・ GitBook Toolchain Documentation](https://toolchain.gitbook.com/plugins/)
* book.jsonにプラグインを登録したら`gitbook install`（npm installが起きる？）

## テストしたもの

* [gitbook-plugin-sharing](https://www.npmjs.com/package/gitbook-plugin-sharing)

  * HTML化されたページ中の共有リンクを消すことができる

* [gitbook-plugin-hide-published-with](https://www.npmjs.com/package/gitbook-plugin-hide-published-with)

  * HTML化されたページ中のPublished with GitBookのリンクを消すことができる

* [gitbook-plugin-graph](https://www.npmjs.com/package/gitbook-plugin-graph)
* [gitbook-plugin-mermaid-gb3](https://www.npmjs.com/package/gitbook-plugin-mermaid-gb3)
* [gitbook-plugin-uml](https://www.npmjs.com/package/gitbook-plugin-uml)

* 日本語は出力されない？

* [gitbook-plugin-puml](https://www.npmjs.com/package/gitbook-plugin-puml)

  * 日本語は文字化ける
  * [When generate chart with non-ascii char are broken. ・ Issue #1 ・ GitbookIO/plugin-puml](https://github.com/GitbookIO/plugin-puml/issues/1)
  * 正確にはpluntuml-encoder側の問題だったようで、それは既に修正されているけど、pumlのほうのpackage.json が対象バージョンを修正していない

a [gitbook-plugin-toc](https://www.npmjs.com/package/gitbook-plugin-toc)

