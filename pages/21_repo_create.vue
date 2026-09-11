<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="リポジトリの作り方 03">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title">Create repositoryを選ぶ</h1>
        <div v-click>
          <p class="deck-subtitle">作成後に確認</p>
          <ul class="deck-lines">
            <li><span class="deck-lines__index">01</span><span>自分たちのリポジトリが開く</span></li>
            <li><span class="deck-lines__index">02</span><span>3つのディレクトリが見える</span></li>
            <li><span class="deck-lines__index">03</span><span>clone用URLを取得できる</span></li>
          </ul>
        </div>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/21-create-repository.jpg" alt="GitHubのCreate repositoryボタン" />
      </figure>
    </div>
  </DeckSlide>
</template>
