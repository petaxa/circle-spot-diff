# 19 リポジトリの作り方 1: テンプレートを開く

- 実装: `../pages/19_repo_template.vue`

## 目的

指定されたテンプレートリポジトリから作業を始める。

## 表示する内容

- 固定見出し「リポジトリの作り方 01」
- URL `https://github.com/petaxa/spot-diff-app`
- 操作「Use this template」から「Create a new repository」を選ぶ
- 画像 `../public/images/19-use-this-template.jpg`

## レイアウト

GitHub画面画像を中央に大きく配置する。タイトル「テンプレートを開く」は一行で表示する。URLは上部へ短く置き、「Use this template」と「Create a new repository」が画像内で読める大きさを確保する。

## 振る舞い

操作箇所の強調を `v-click` で表示する。

## 出典

- [petaxa/spot-diff-app](https://github.com/petaxa/spot-diff-app)

## 維持すること

Forkではなく、`Use this template`を使うことを明確にする。
