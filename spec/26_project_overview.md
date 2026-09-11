# 26 デモプロジェクトの全体像

- 実装: `../pages/26_project_overview.vue`

## 目的

デモプロジェクト「Taskly」が何をするアプリで、どの技術で構成されているかを把握する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 01」
- 主題「Tasklyは、毎日のタスクを管理するToDoアプリ」
- フロントエンド「Vue + Vue Router + Vize」
- バックエンド「Hono REST API」
- 補足「フロントエンドとバックエンドは、独立したViteアプリ」
- 画像 `../public/images/26-taskly-overview.jpg`

## レイアウト

Tasklyの実画面を中央から右へ大きく置く。主題と技術構成は左側へ短く置き、画面の存在感を主にする。

## 振る舞い

フロントエンド、バックエンドの順に `v-click` で表示する。

## 出典

- [spot-diff-app README](https://github.com/petaxa/spot-diff-app/blob/main/README.md)

## 維持すること

機能一覧は次ページへ分け、このページではアプリの役割と技術構成だけを扱う。
