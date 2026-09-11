<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRの作り方" variant="statement">
    <div class="deck-centered">
      <p class="deck-statement">1つのPRでは、<br /><strong>1つのバグ修正だけ</strong>を扱う</p>
      <p class="deck-note">別の問題は同じPRに混ぜず、記録して別のPRで扱う</p>
    </div>
  </DeckSlide>
</template>
