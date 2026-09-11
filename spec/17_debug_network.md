# 17 ブラウザの通信履歴を確認する

- 実装: `../pages/17_debug_network.vue`

## 目的

フロントエンドとAPIの間で何が起きたかを、DevToolsのNetworkから確認する。

## 表示する内容

- 固定見出し「バグの調査方法 03」
- 主題「Networkで、送信内容とAPIの返答を確認する」
- 手順
  1. Networkタブを開き、Fetch/XHRに絞る
  2. 問題を再現して対象の通信を選ぶ
  3. Request、Status、Responseを確認する
- 補足「通信が見つからない場合は、フロントエンド側で処理が止まっている可能性がある」
- 画像 `../public/images/17-chrome-devtools-network.jpg`
- 補助画像 `../public/images/17-chrome-devtools-response.jpg`

## レイアウト

Chrome DevToolsのNetwork一覧を中央に大きく置く。Responseタブの画像は右下へ重ねず、クリック後に同じ位置へ切り替えて表示する。Request、Status、Responseの位置を画像の外側から細い線とラベルで示す。

## 振る舞い

最初にNetwork一覧を表示する。RequestとStatusを強調したあと、`v-click` でResponseタブの画像へ切り替える。

## 出典

- [Chrome DevTools: Inspect network activity](https://developer.chrome.com/docs/devtools/network)

## 維持すること

通信内容に認証情報がある場合は画面共有しない。Consoleとの役割の違いが伝わる内容にする。
