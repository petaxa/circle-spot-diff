<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="開発環境のセットアップ 02" title="プロジェクトへ移動する">
    <div class="deck-command-stack">
      <CommandBlock command="cd <repository>" class="deck-command-card--wide" />
      <p class="deck-note">このあとのコマンドは、プロジェクトのルートで実行する</p>
    </div>
  </DeckSlide>
</template>
