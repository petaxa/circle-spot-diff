<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";

const frontendChecks = `vp run -F @taskly/frontend vize:fmt
vp run -F @taskly/frontend vize:fmt:fix
vp run -F @taskly/frontend vize:lint
vp run -F @taskly/frontend vize:check`;
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 05">
    <template #title><span class="project-checks-title">ソースコードの問題を見つけるコマンド</span></template>
    <div class="deck-stack" style="gap: 0.7rem">
      <div class="deck-check-grid">
        <div v-click="1" class="deck-check-grid__item">共通チェック<br /><span class="deck-inline-code">vp check</span></div>
        <div v-click="1" class="deck-check-grid__item">全チェック<br /><span class="deck-inline-code">vp run check:all</span></div>
        <div v-click="3" class="deck-check-grid__item">テスト<br /><span class="deck-inline-code">vp test</span></div>
      </div>
      <pre v-click="2" class="deck-code-panel" style="font-size: 0.86rem"><code>{{ frontendChecks }}</code></pre>
    </div>
  </DeckSlide>
</template>

<style scoped>
.project-checks-title {
  font-size: 2.5rem;
  white-space: nowrap;
}
</style>
