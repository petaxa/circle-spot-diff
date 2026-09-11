# 30 ソースコードの問題を見つけるコマンド

- 実装: `../pages/30_project_checks.vue`

## 目的

静的解析、型チェック、テストを使い、ソースコードの問題を見つける入口を把握する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 05」
- タイトル「ソースコードの問題を見つけるコマンド」
- 共通チェック `vp check`
- 全チェック `vp run check:all`
- フロントエンド個別チェック

```bash
vp run -F @taskly/frontend vize:fmt
vp run -F @taskly/frontend vize:fmt:fix
vp run -F @taskly/frontend vize:lint
vp run -F @taskly/frontend vize:check
```

- テスト `vp test`

## レイアウト

共通チェック、全チェック、テストを上部の3列に置く。フロントエンド個別コマンドをその下のコードブロックへまとめる。長いタイトルは一行で表示し、フッターとの間に余白を残す。

## 振る舞い

「共通」「フロントエンド個別」「テスト」の順に `v-click` で表示する。

## 出典

- [spot-diff-app README](https://github.com/petaxa/spot-diff-app/blob/main/README.md)

## 維持すること

コマンド名を省略して別名にしない。`vize:fmt`と`vize:fmt:fix`の違いが見分けられるようにする。
