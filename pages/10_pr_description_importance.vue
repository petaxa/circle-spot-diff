<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRの作り方">
    <div class="deck-stack" style="gap: 0.8rem">
      <h1 class="deck-body-title" style="font-size: 2.15rem; white-space: nowrap">Descriptionは、修正の背景と確認方法を共有する場所</h1>
      <div class="deck-image-layout deck-image-layout--balanced">
        <div class="deck-image-copy">
          <p class="deck-note">変更コードを読む前に、何を確認すればよいか分かる状態にする</p>
        </div>
        <figure class="deck-image-frame" style="height: 17.5rem">
          <img src="/images/12-pull-request-description.jpg" alt="Pull RequestのDescription記入例" />
        </figure>
      </div>
    </div>
  </DeckSlide>
</template>
