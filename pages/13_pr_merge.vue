<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRのマージ">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <ol class="deck-steps">
          <li v-click><span class="deck-steps__index">01</span><span>レビュー結果と自動チェックを確認</span></li>
          <li v-click><span class="deck-steps__index">02</span><span>未解決のコメントがないことを確認</span></li>
          <li v-click><span class="deck-steps__index">03</span><span>Merge pull requestを選び、確定</span></li>
        </ol>
        <p class="deck-note">マージ後は不要になった作業ブランチを削除する</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--screen">
        <img src="/images/13-merge-pull-request.jpg" alt="GitHubのMerge pull request操作画面" />
      </figure>
    </div>
  </DeckSlide>
</template>
