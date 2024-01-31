# このプロジェクトについて

Nuxt3を用いたテンプレートリポジトリです。

## 開発環境構築方法

```bash
pnpm install
pnpm dev
```

[http://localhost:3000](http://localhost:3000)にアクセスしてください。

## Node と pnpm のバージョンについて

volta で固定しています。

このプロジェクトを使用する場合は [volta](https://volta.sh/) のセットアップを先に行ってください。

セットアップに関しましては、こちらの記事を参考にしてください

https://zenn.dev/xeiculy/articles/03871845342228

## CodeRabbitについて

CodeRabbitによるレビューを受けたい場合は、CadeRabbitのサイトから設定を行う。

特に使用しない場合は、coderabbitの設定ファイルである`coderabbit.yaml`は削除してください。

## 技術構成について

| 技術/ツール       | 説明                                             |
| ----------------- | ------------------------------------------------ |
| Nuxt3             | Vue3ベースのフレームワーク                       |
| Tailwind CSS      | CSSフレームワーク                                |
| TypeScript        | 静的型付けが特徴で、JavaScriptのスーパーセット   |
| husky/lint-staged | コミット時に任意のコマンドを自動実行できるツール |
| NuxtUI            | UIコンポーネントライブラリ                       |
| pnpm              | Nodeパッケージマネージャ                         |
| volta             | Nodeなどのバージョン管理ツール                   |
| Prettier          | コードフォーマッター                             |
| ESLint            | コード書き方をチェックするツール                 |
| vitest            | テスティングフレームワーク                       |
| coderabbit        | AIレビューツール                                 |

バージョンの詳細や、その他のツールについては`package.json`を参照してください。

## ディレクトリ構成のイメージ

```sh
src/
├── assets/
├── components/
├── composable/
├── layout/
├── lib/
├── middleware/
├── pages/
├── plugins/
├── public/
├── store/
├── types/
└── utils/
```

| ディレクトリ | 説明                                                                                                                          |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| .husky       | huskyの設定ファイルを管理                                                                                                     |
| .vscode      | VSCodeの設定ファイルと推奨拡張機能ファイルを管理                                                                              |
| assets       | 画像ファイルなどやCSSファイルを管理                                                                                           |
| components   | ページに表示するものやコンポーネントを管理                                                                                    |
| composable   | [Composition API](https://v3.vuejs.org/guide/composition-api-introduction.html)を使用した論理的な関数（コンポーザブル）を格納 |
| layout       | アプリケーションのレイアウト定義                                                                                              |
| lib          | ライブラリに依存した関数（初期設定など）を管理                                                                                |
| middleware   | ページやグループのページがレンダリングされる前に実行されるカスタム関数を格納                                                  |
| pages        | アプリケーションのページコンポーネントを格納                                                                                  |
| plugins      | Vueインスタンスが初期化される際に実行されるべきグローバルなプラグインやライブラリの初期化スクリプトを格納                     |
| public       | ファビコンなど変更されない静的ファイルを格納                                                                                  |
| store        | [Pinia](https://pinia.vuejs.org/)を使用したグローバルステート管理のためのストアを格納                                         |
| types        | グローバルに使用可能な型を管理                                                                                                |
| utils        | 汎用的に使える関数を管理                                                                                                      |
