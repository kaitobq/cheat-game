# セットアップ

1. 依存関係のインストール

   `npm i`

3. 必要なESLint関連のパッケージのインストール

   `npm install --save-dev eslint eslint-config-next eslint-config-prettier eslint-plugin-tailwindcss @typescript-eslint/parser @typescript-eslint/eslint-plugin`

   • eslint: ESLint本体

   • eslint-config-next: Next.js向けのESLint設定

   • eslint-config-prettier: ESLintとPrettierの競合を防ぐための設定

   • eslint-plugin-tailwindcss: Tailwind CSSのクラス名の検証を行うプラグイン

   • @typescript-eslint/parser: TypeScriptを解析するためのESLint用パーサー

   • @typescript-eslint/eslint-plugin: TypeScript向けのESLintルールを提供

5. 必要なPrettier関連のパッケージのインストール

   `npm install --save-dev prettier prettier-plugin-organize-imports`

   • prettier: コードフォーマッター本体

   • prettier-plugin-organize-imports: import文を整理するためのPrettierプラグイン

7. その他の開発ツール

   `npm install --save-dev npm-run-all husky lint-staged @commitlint/cli @commitlint/config-conventional`

   • npm-run-all: 複数の npm スクリプトを並列または直列で実行するツール。

   • Husky: Git フック管理ツール。

   • Lint-staged: コミット前に特定のファイルに対してのみリンティングを実行。

   • Commitlint: コミットメッセージのフォーマットをチェック。

## 開発環境構築参考

https://zenn.dev/siakas/articles/05481bdefacd13

https://qiita.com/mu-suke08/items/43a492fda5cd71a31506#1-husky%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB

https://typicode.github.io/husky/get-started.html

https://zenn.dev/risu729/articles/latest-husky-lint-staged

https://zenn.dev/kalubi/articles/27fa889c338cdf#commitlint-%E5%B0%8E%E5%85%A5%E6%96%B9%E6%B3%95

# コミットメッセージの規約について

**コミットメッセージののフォーマット**

`<type>: <subject>`

1. type (必須)

   • コミットの目的を明確にするための短いラベルです。

   • 使用可能なタイプ:

   • feat: 新機能の追加

   • fix: バグ修正

   • docs: ドキュメントの変更 (コードは変更しない)

   • style: コードのフォーマット変更 (動作に影響しない)

   • refactor: コードのリファクタリング (バグ修正や新機能の追加を含まない)

   • test: テストの追加または修正

   • chore: ビルドプロセスや補助ツールの変更 (コードやテストには影響しない)

   • perf: パフォーマンス向上のための変更

3. subject (必須)

   • 変更内容を簡潔に説明する短い文。

   • 最大50文字程度に収めることを推奨します。

   • 動詞の現在形を使用します (例: Add, Fix, Update)。
