# 21 リポジトリの作り方 3: 作成を完了する

- 実装: `../pages/21_repo_create.vue`

## 目的

テンプレートから新しいリポジトリを作成し、ローカル環境構築へ進める状態にする。

## 表示する内容

- 固定見出し「リポジトリの作り方 03」
- 操作「Create repository」を選ぶ
- 完了条件
  - 作成したリポジトリのトップページが開く
  - `frontend`、`backend`、`documentation`が見える
  - clone用URLを取得できる
- 画像 `../public/images/21-create-repository.jpg`

## レイアウト

GitHubの作成フォーム画像を中央に大きく置き、入力済みのRepository nameと「Create repository」ボタンを読める大きさにする。完了条件は画像の横へ短く添える。

## 振る舞い

右側の完了状態を `v-click` で表示する。

## 維持すること

テンプレート元ではなく、自分たちが作成したリポジトリにいることを確認させる。
