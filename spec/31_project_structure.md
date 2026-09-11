# 31 プロジェクトの構成

- 実装: `../pages/31_project_structure.vue`

## 目的

調査対象がフロントエンド、バックエンド、システム仕様書のどこにあるか判断できるようにする。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 06」

```text
.
├── frontend/       Vue + Vue Router + Vize
├── backend/        Hono REST API
└── documentation/  Ox Contentのシステム仕様書
```

- 補足「画面の問題は`frontend/`、APIの問題は`backend/`から調べる」

## レイアウト

ディレクトリツリーを中央のコードブロックに大きく置く。補足は下側へ置く。

## 振る舞い

なし。

## 出典

- [spot-diff-app README](https://github.com/petaxa/spot-diff-app/blob/main/README.md)

## 維持すること

ツリーを細かく展開しすぎない。調査を始める場所を選べる粒度に留める。
