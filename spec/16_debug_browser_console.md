# 16 ブラウザコンソールを確認する

- 実装: `../pages/16_debug_browser_console.vue`

## 目的

画面側の問題を疑うとき、DevToolsのConsoleでJavaScriptエラーと警告を確認する。

## 表示する内容

- 固定見出し「バグの調査方法 02」
- 主題「Consoleの赤いエラーから、失敗した場所を探す」
- 手順
  1. ブラウザのDevToolsを開く
  2. Consoleタブを選ぶ
  3. 問題を再現し、最初の赤いエラーを確認する
- 確認する情報「エラーメッセージ」「ファイル名」「行番号」
- 画像 `../public/images/16-chrome-devtools-console.jpg`

## レイアウト

Chrome DevToolsのConsole画像を主役として中央から右へ大きく置く。赤いエラー行と右端の発生元を読める大きさにする。3つの手順は左側へ短く添える。

## 振る舞い

手順を `v-click` で一つずつ表示する。

## 出典

- [Chrome DevTools: Console overview](https://developer.chrome.com/docs/devtools/console)

## 維持すること

警告をすべて直す話へ広げず、再現操作に対応する最初のエラーを追うことに集中する。
