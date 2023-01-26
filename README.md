# はじめに

## [HonkitTemplate](https://github.com/dtxmuramasa/HonkitTemplate)とは
- [Honkit](https://github.com/honkit/honkit)でプログラムの仕様書や設計書を作成するために必要なツール、プラグインをバンドルしたプロジェクトのテンプレートです。
- もともとは[GitbookTemplate](https://github.com/dtxmuramasa/GitbookTemplate)でしたが、本体の[Gitbook](https://github.com/GitbookIO/gitbook)がLegacyとなり新しい環境に導入できなくなったため、Forkされた[Honkit](https://github.com/honkit/honkit)に差し替えたものになります。[azu](https://twitter.com/azu_re)様、ありがとうございます！

## 注意事項
- [本テンプレート](https://github.com/dtxmuramasa/HonkitTemplate)は日本語プロジェクトでの使用しか考慮していません。
	- This template is only considered for use in Japanese projects.
- 本テンプレートはWindows環境に合わせて作成しています。
- [Honkit](https://github.com/honkit/honkit)の成り立ちから、ところどころにGitbookの表記があります。


## ドキュメント生成環境構築手順
- 詳しくは[ドキュメント生成環境構築](./src/StructEnvironments/BuildDocument.md)をご覧ください。


## ドキュメントの生成、更新コマンド

```
$ npm run build
```

## ドキュメント閲覧サーバ起動コマンド
- 下記コマンド実行後、[http://localhost:4000](http://localhost:4000)で確認できます。

```
$ npm run serve
```

## 導入プラグイン
- まだ[Honkit](https://github.com/honkit/honkit)に移行後、完全な互換性があるか確認できていません。
- hide-published-with
	- https://www.npmjs.com/package/gitbook-plugin-hide-published-with
	- Gitbookへのpublishボタンを消します。
	- リポジトリなどは残っていないが、機能はする模様。
- -lunr, -search
	- https://www.npmjs.com/package/gitbook-plugin-lunr
	- https://www.npmjs.com/package/gitbook-plugin-search
	- 標準搭載されている検索エンジンを無効化します。
- search-pro-kui
	- https://www.npmjs.com/package/gitbook-plugin-search-pro-kui
	- あらゆるutf-8文字の検索に高度に対応した検索エンジンプラグイン。
	- これを導入しないと日本語の部分検索が一部うまくいかないことがある。
		- 例えば「環境構築」での検索で引っかかる文書が「構築」では引っかからなかったりなど。
- uml
	- https://www.npmjs.com/package/gitbook-plugin-uml
	- plantUMLを扱うためのプラグイン。
- expandable-chapters
	- https://www.npmjs.com/package/gitbook-plugin-expandable-chapters
	- サイドバーのメニューをCollapse/Expandできるツリービューにするプラグイン。
- include-codeblock
	- https://www.npmjs.com/package/gitbook-plugin-include-codeblock
	- ファイルの内容を展開してくれるマクロを提供するプラグイン。
- code-editor
	- https://www.npmjs.com/package/gitbook-plugin-code-editor
	- よくあるコードエディタとコードの実行結果が見られるアレ。
- code
	- https://www.npmjs.com/package/gitbook-plugin-code
	- 複数行のコード記述に行数を表示してくれるプラグイン。

## ライセンス
- 本テンプレートは[Honkit](https://github.com/honkit/honkit)のライセンスに準じています。
- [Apache License 2.0全文](https://github.com/dtxmuramasa/HonkitTemplate/blob/main/LICENSE)
