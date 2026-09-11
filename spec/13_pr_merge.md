# 13 PRのマージ方法

- 実装: `../pages/13_pr_merge.vue`

## 目的

レビューと確認が終わったPRを、安全に`main`へ取り込む流れを理解する。

## 表示する内容

- 固定見出し「PRのマージ」
- 手順01「レビュー結果と自動チェックを確認する」
- 手順02「未解決のコメントがないことを確認する」
- 手順03「Merge pull request を選び、マージを確定する」
- 補足「マージ後は不要になった作業ブランチを削除する」
- 画像 `../public/images/13-merge-pull-request.jpg`

## レイアウト

GitHubのマージ操作画像を中央から右へ大きく置く。3つの確認手順は左側に短く並べ、補足は下端に置く。

## 振る舞い

3つの手順を `v-click` で順番に表示する。

## 出典

- [GitHub Docs: Merging a pull request](https://docs.github.com/en/pull-requests/how-tos/merge-and-close-pull-requests/merging-a-pull-request)

## 維持すること

承認やチェックを省略してマージできるように見せない。具体的なマージ方式はリポジトリのルールに従う。
