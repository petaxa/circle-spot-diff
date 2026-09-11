<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="リポジトリの作り方 02">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title">作成内容を入力する</h1>
        <ol class="deck-steps">
          <li v-click><span class="deck-steps__index">01</span><span>Owner</span></li>
          <li v-click><span class="deck-steps__index">02</span><span>Repository name</span></li>
          <li v-click><span class="deck-steps__index">03</span><span>Visibility</span></li>
        </ol>
        <p class="deck-note">OwnerとVisibilityは当日の案内に合わせ、Repository nameはチーム内で共有する</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/20-repository-settings.jpg" alt="GitHubの新規リポジトリ設定画面" />
      </figure>
    </div>
  </DeckSlide>
</template>
