# 29 開発で使う主なコマンド

- 実装: `../pages/29_project_commands.vue`

## 目的

起動、ビルド、仕様書の確認に使うプロジェクト共通コマンドを把握する。

## 表示する内容

- 固定見出し「デモプロジェクトの基礎知識 04」
- コマンドと用途

```bash
vp run dev:all    # フロントエンドとバックエンドを起動
vp run build:all  # アプリと仕様書をビルド
vp run docs:dev   # システム仕様書を起動
vp run docs:build # システム仕様書をビルド
```

## レイアウト

4行のコマンドを中央のコードブロックにまとめ、右側のコメントで用途を対応させる。

## 振る舞い

なし。

## 出典

- [spot-diff-app README](https://github.com/petaxa/spot-diff-app/blob/main/README.md)

## 維持すること

セットアップで説明済みの`dev:all`は、ここでは他コマンドとの位置づけを示すために載せる。
