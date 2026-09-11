# 20 リポジトリの作り方 2: 作成内容を入力する

- 実装: `../pages/20_repo_settings.vue`

## 目的

チームの作業先として識別できるリポジトリ名と公開範囲を設定する。

## 表示する内容

- 固定見出し「リポジトリの作り方 02」
- 入力項目「Owner」「Repository name」「Visibility」
- 補足「OwnerとVisibilityは、当日の案内に合わせる」
- 補足「Repository nameはチーム内で共有する」
- 画像 `../public/images/20-repository-settings.jpg`

## レイアウト

GitHubの作成フォーム画像を中央から右へ大きく置く。Owner、Repository name、Visibilityが一画面に収まる状態を見せ、確認する3項目は左側へ短く並べる。

## 振る舞い

入力項目を `v-click` で一つずつ表示する。

## 維持すること

公開範囲を推測で指定しない。参加者が後でcloneできるOwnerに作成することを優先する。
