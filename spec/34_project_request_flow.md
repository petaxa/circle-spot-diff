# 34 画面操作からAPI応答までの流れ

- 実装: `../pages/34_project_request_flow.vue`

## 目的

画面操作を起点に、フロントエンド、API、バックエンドをどの順で処理が通るか理解する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 09」
- 処理順
  1. `frontend/src/views/`の画面が操作を受け取る
  2. `frontend/src/api/todos.ts`の関数を呼ぶ
  3. ブラウザが`http://127.0.0.1:8787/api`へリクエストを送る
  4. `backend/src/index.ts`のHonoルートが処理する
  5. インメモリのデータを読み書きし、JSONを返す
  6. 画面がレスポンスを反映する
- 補足「止まった段階に合わせて、Console、Network、バックエンドログを確認する」

## レイアウト

6段階を一本の水平フローとして一列に押し込まず、前半3段階と後半3段階の二段に分ける。接続線は処理方向だけを示す。

## 振る舞い

6段階を `v-click` で順番に表示する。最後に補足を表示する。

## 出典

- [frontend/src/views/TodosView.vue](https://github.com/petaxa/spot-diff-app/blob/main/frontend/src/views/TodosView.vue)
- [frontend/src/api/todos.ts](https://github.com/petaxa/spot-diff-app/blob/main/frontend/src/api/todos.ts)
- [backend/src/index.ts](https://github.com/petaxa/spot-diff-app/blob/main/backend/src/index.ts)

## 維持すること

具体的なバグの答えは載せない。調査時に辿る順序だけを示す。
