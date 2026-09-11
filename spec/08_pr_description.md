# 08 PRの作り方 3: PR作成画面

- 実装: `../pages/08_pr_description.vue`

## 目的

Pushした作業ブランチから、GitHubのPull Request作成画面を開く手順を理解する。

## 表示する内容

- 固定見出し「PRの作り方 03」
- タイトル「PR作成画面を開く」
- 手順01「GitHubでリポジトリを開く」
- 手順02「Compare & pull requestを選ぶ」
- 補足「バナーが表示されない場合は、ブランチ一覧から作業ブランチを開く」
- 画像 `../public/images/11-compare-pull-request-banner.jpg`
- 画像 `../public/images/11-branch-dropdown.jpg`

## レイアウト

左側に2つの手順を並べる。右側は、通常使うCompare & pull requestのバナーを上へ大きく置き、代替の入口となるブランチ一覧を下へ置く。

## 振る舞い

2つの手順を `v-click` で順番に表示する。画像は最初から表示する。

## 出典

- [GitHub Docs: Creating a pull request](https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request)

## 維持すること

Descriptionの入力前に、作業ブランチからPR作成画面へ移動する順序を保つ。通常ルートと代替ルートの優先度を逆転させない。
