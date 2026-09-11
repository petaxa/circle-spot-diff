# 22 開発環境のセットアップ 1: Clone

- 実装: `../pages/22_setup_clone.vue`

## 目的

作成したGitHubリポジトリをローカルへcloneする。

## 表示する内容

- 固定見出し「開発環境のセットアップ 01」
- タイトル「リポジトリをcloneする」
- コマンド `git clone https://github.com/<owner>/<repository>.git`
- 補足「URLは、自分たちが作成したリポジトリのCodeメニューからコピーする」
- 画像 `../public/images/22-code-clone-url.jpg`

## レイアウト

GitHubのCodeメニュー画像を中央から右へ大きく置き、HTTPSのclone URLとコピーボタンを読める大きさにする。コマンドは左側へ短く置く。

## 振る舞い

なし。

## 維持すること

テンプレート元のURLをclone例に使わない。`<owner>`と`<repository>`が置換箇所だと分かる表現にする。
