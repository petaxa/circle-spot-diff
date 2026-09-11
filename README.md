# __DECK_TITLE__

Slidev で作るプレゼンテーションです。

## 開発

```bash
__INSTALL_COMMAND__
__DEV_COMMAND__
```

`slides.md` がスライド順を管理し、各ページの実装は `pages/` に置きます。
ページごとの意図は、同名の `spec/*.md` に記録します。共通の見た目は `layouts/`、`components/`、`styles/` に分かれています。

デザインを変更・拡張するときは、最初に [DESIGN.md](./DESIGN.md) を確認してください。

LLM にスライドを書かせる場合は、[AGENTS.md](./AGENTS.md) の指示に従い、`DESIGN.md` と対象ページの `spec/*.md` を読ませてください。

## 主なコマンド

```bash
__DEV_COMMAND__
__BUILD_COMMAND__
__EXPORT_COMMAND__
```

`export` には環境によって Playwright のブラウザ導入が必要です。

## GitHub Pages へのデプロイ

`main` または `master` ブランチへ push すると、`.github/workflows/deploy.yml` が Slidev をビルドして GitHub Pages へデプロイします。手動実行にも対応しています。

workflow は lockfile から npm / pnpm / Yarn / Bun を判定します。通常のリポジトリでは `/<repository-name>/`、`*.github.io` リポジトリでは `/` をベースパスとして自動設定します。

GitHub リポジトリの **Settings → Pages → Build and deployment → Source** が **GitHub Actions** になっていることを確認してください。Vercel や Netlify の設定ファイルは使用しません。
