# 28 タスクの見方

- 実装: `../pages/28_project_view_features.vue`

## 目的

Tasklyが、タスクの一覧だけでなく進捗や期限を複数の見方で表示することを把握する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 03」
- 表示「タスクリスト」「ガントチャート」「バーンダウンチャート」
- 集計「全タスクを基準にした進捗と期限のサマリー」
- 絞り込み「キーワードと完了状態」
- 画像 `../public/images/28-taskly-list.png`
- 画像 `../public/images/28-taskly-gantt-new.png`
- 画像 `../public/images/28-taskly-burndown-new.png`
- 画像 `../public/images/28-taskly-summary-crop.png`
- 画像 `../public/images/28-taskly-filter.png`

## レイアウト

実画面画像を大きく使う。左側には機能名だけの段階リストを置き、「タスクリスト」「ガントチャート」「バーンダウンチャート」「集計」「絞り込み」を順に追加する。同じタイミングで右側の画像を対応する実画面へ切り替える。

## 振る舞い

最初にタスクリストを表示する。`v-click`ごとにガントチャート、バーンダウンチャート、集計、絞り込みの項目を追加し、画像も同じ順序で切り替える。

## 出典

- [spot-diff-app README](https://github.com/petaxa/spot-diff-app/blob/main/README.md)

## 維持すること

機能を追加で推測しない。READMEに記載された表示、集計、絞り込みだけを扱う。各項目と画像の内容を一致させる。
