<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRの作り方 01" title="作業ブランチを作る">
    <div class="deck-command-stack">
      <CommandBlock command="git switch -c fix/<短い名前>" class="deck-command-card--wide" />
      <p class="deck-note">このブランチで変更をコミットする</p>
    </div>
  </DeckSlide>
</template>
