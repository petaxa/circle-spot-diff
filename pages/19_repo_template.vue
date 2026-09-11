<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="リポジトリの作り方 01">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title" style="font-size: 1.85rem; white-space: nowrap">テンプレートを開く</h1>
        <p class="deck-subtitle deck-inline-code">github.com/petaxa/spot-diff-app</p>
        <p v-click class="deck-callout">Use this template<br />→ Create a new repository</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/19-use-this-template.jpg" alt="GitHubのUse this templateメニュー" />
      </figure>
    </div>
  </DeckSlide>
</template>
