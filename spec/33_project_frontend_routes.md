# 33 フロントエンドのルーティング定義

- 実装: `../pages/33_project_frontend_routes.vue`

## 目的

画面URLとVueコンポーネントの対応を、どのファイルで確認できるか把握する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 08」
- 主題「ルーティング定義は `frontend/src/router.ts`」
- 対応
  - `/` は `/tasks` へリダイレクト
  - `/tasks` は `TodosView`
  - `/tasks/:id` は `TodoDetailView`
  - その他は `NotFoundView`
- 補足「`frontend/src/main.ts`でrouterをVueアプリへ登録する」

## レイアウト

ファイル名を上部に大きく置き、その下にパスとコンポーネントの対応を4行で並べる。パス列は`/tasks/:id`がコンポーネント名へ重ならない幅を確保する。補足は下端に置く。

## 振る舞い

4つのルートを `v-click` で一行ずつ表示する。

## 出典

- [frontend/src/router.ts](https://github.com/petaxa/spot-diff-app/blob/main/frontend/src/router.ts)
- [frontend/src/main.ts](https://github.com/petaxa/spot-diff-app/blob/main/frontend/src/main.ts)

## 維持すること

実ファイルの定義をそのまま扱い、正しいはずのURLを推測で補正しない。このページではバグの場所を指摘しない。
