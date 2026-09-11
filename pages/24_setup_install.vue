<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
import InstallTabs from "../components/InstallTabs.vue";
</script>

<template>
  <DeckSlide section-label="開発環境のセットアップ 03" title="依存関係をインストールする">
    <div class="deck-stack">
      <InstallTabs />
      <p class="deck-note">どれか一つだけ実行する</p>
    </div>
  </DeckSlide>
</template>
