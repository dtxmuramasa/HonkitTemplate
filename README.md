# はじめに

## GitbookTemplateとは
- Gitbookでプログラムの仕様書や設計書を作成するために必要なツール、プラグインをバンドルしたプロジェクトのテンプレートです。
- 日本語プロジェクトでの使用しか考慮していません。
	- This template is only considered for use in Japanese projects.

## 注意事項
- 本ドキュメントは[Gitbook](https://github.com/GitbookIO/gitbook)を用いて生成しています。
- 本ドキュメントの更新には[Gitbook](https://github.com/GitbookIO/gitbook)が必要です。
	- [Gitbook](https://github.com/GitbookIO/gitbook)の利用には[Node.js](https://nodejs.org/ja/)が必要です。


## ドキュメント生成環境構築手順
1. 下記コマンドを実行します。

```
$ bash provision.sh
```

- 詳しくは[ドキュメント生成環境構築](./src/StructEnvironments/BuildDocument.md)をご覧ください。


## ドキュメントの生成、更新コマンド

``` bash:command
$ npm run build
```

## ドキュメント閲覧サーバ起動コマンド
- 下記コマンド実行後、[http://localhost:4000](http://localhost:4000)で確認できます。

``` bash:command
$ npm run serve
```

## 導入プラグイン
- -sharing
	- https://www.npmjs.com/package/gitbook-plugin-sharing
	- 各種SNSのシェアボタンを消します。
- hide-published-with
	- https://www.npmjs.com/package/gitbook-plugin-hide-published-with
	- Gitbookへのpublishボタンを消します。
	- リポジトリなどは残っていないが、機能はする模様。
- -lunr, -search
	- https://www.npmjs.com/package/gitbook-plugin-lunr
	- https://www.npmjs.com/package/gitbook-plugin-search
	- Gitbookに標準搭載されている検索エンジンを無効化します。
- search-pro-kui
	- https://www.npmjs.com/package/gitbook-plugin-search-pro-kui
	- あらゆるutf-8文字の検索に高度に対応した検索エンジンプラグイン。
	- これを導入しないと日本語の部分検索が一部うまくいかないことがある。
		- 例えば「環境構築」での検索で引っかかる文書が「構築」では引っかからなかったりなど。
- uml
	- https://www.npmjs.com/package/gitbook-plugin-uml
	- Gitbook用のplantUMLプラグイン。
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
