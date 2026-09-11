<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="開発環境のセットアップ 04" title="アプリを起動する">
    <div class="deck-command-stack">
      <CommandBlock command="vp run dev:all" class="deck-command-card--wide" />
      <div v-click class="deck-split">
        <div class="deck-split__column">
          <h2 class="deck-split__title">フロントエンド</h2>
          <p class="deck-split__text deck-inline-code">http://127.0.0.1:5173</p>
        </div>
        <div class="deck-split__column">
          <h2 class="deck-split__title">バックエンド</h2>
          <p class="deck-split__text deck-inline-code">http://127.0.0.1:8787</p>
        </div>
      </div>
    </div>
  </DeckSlide>
</template>
