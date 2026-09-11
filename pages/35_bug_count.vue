<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="HANDS-ON" variant="statement">
    <div class="deck-centered">
      <p class="deck-statement" style="font-size: 2.8rem">このアプリに潜んでいるバグは</p>
      <div v-click class="deck-number-reveal">
        <span class="deck-number-reveal__number">12</span><span class="deck-number-reveal__unit">個</span>
      </div>
    </div>
  </DeckSlide>
</template>
