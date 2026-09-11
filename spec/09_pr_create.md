# 09 PRの作り方 4: Descriptionと作成

- 実装: `../pages/09_pr_create.vue`

## 目的

PR作成画面で対象ブランチを確認し、Descriptionを書いてからPull Requestを作成する操作を理解する。

## 表示する内容

- 固定見出し「PRの作り方 04」
- タイトル「Descriptionを書いて作成する」
- 手順01「baseが `main`、compareが作業ブランチであることを確認する」
- 手順02「TitleとDescriptionへ、修正内容と確認方法を書く」
- 手順03「Create pull requestを選ぶ」
- 画像 `../public/images/09-create-pull-request-form.png`

## レイアウト

左側に3つの操作を順番に並べ、右側にDescription入力欄とCreate pull requestボタンが同時に見えるGitHub画面を大きく置く。

## 振る舞い

3つの手順を `v-click` で順番に表示する。画像は最初から表示する。

## 出典

- [GitHubのPull Requestでtemplateを使ってみた](https://0222-nnn.com/blog/20250823_github_pullrequest_template/)

## 維持すること

ブランチの確認、Descriptionの入力、作成ボタンの順序を保つ。GUI操作を画面画像なしで説明しない。
