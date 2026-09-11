<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 08">
    <div class="deck-stack">
      <h1 class="deck-body-title">ルーティング定義は<br /><span class="deck-inline-code">frontend/src/router.ts</span></h1>
      <dl class="deck-term-list">
        <div v-click class="deck-term-list__row"><dt class="deck-inline-code">/</dt><dd><span class="deck-inline-code">/tasks</span>へリダイレクト</dd></div>
        <div v-click class="deck-term-list__row"><dt class="deck-inline-code">/tasks</dt><dd>TodosView</dd></div>
        <div v-click class="deck-term-list__row"><dt class="deck-inline-code">/tasks/:id</dt><dd>TodoDetailView</dd></div>
        <div v-click class="deck-term-list__row"><dt>その他</dt><dd>NotFoundView</dd></div>
      </dl>
      <p class="deck-note"><span class="deck-inline-code">frontend/src/main.ts</span> でrouterをVueアプリへ登録する</p>
    </div>
  </DeckSlide>
</template>

<style scoped>
.deck-term-list__row {
  grid-template-columns: 9rem minmax(0, 1fr);
}
</style>
