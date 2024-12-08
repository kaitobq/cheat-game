# For Contributer

1. 依存関係のインストール
   `npm i`

2. 必要なESLint関連のパッケージのインストール
   `npm install --save-dev eslint eslint-config-next eslint-config-prettier eslint-plugin-tailwindcss @typescript-eslint/parser @typescript-eslint/eslint-plugin`
   • eslint: ESLint本体
   • eslint-config-next: Next.js向けのESLint設定
   • eslint-config-prettier: ESLintとPrettierの競合を防ぐための設定
   • eslint-plugin-tailwindcss: Tailwind CSSのクラス名の検証を行うプラグイン
   • @typescript-eslint/parser: TypeScriptを解析するためのESLint用パーサー
   • @typescript-eslint/eslint-plugin: TypeScript向けのESLintルールを提供

3. 必要なPrettier関連のパッケージのインストール
   `npm install --save-dev prettier prettier-plugin-organize-imports`
   • prettier: コードフォーマッター本体
   • prettier-plugin-organize-imports: import文を整理するためのPrettierプラグイン

4. その他の開発ツール
   `npm install --save-dev npm-run-all husky lint-staged @commitlint/cli @commitlint/config-conventional`
   • npm-run-all: 複数の npm スクリプトを並列または直列で実行するツール。
   • Husky: Git フック管理ツール。
   • Lint-staged: コミット前に特定のファイルに対してのみリンティングを実行。
   • Commitlint: コミットメッセージのフォーマットをチェック。
