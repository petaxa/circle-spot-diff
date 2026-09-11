<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";

const log = `POST /api/todos 500  14ms
ValidationError: title is required
    at backend/src/index.ts:84:12`;
</script>

<template>
  <DeckSlide class="slide-15" section-label="バグの調査方法 01" title="操作の直後に、バックエンドのログを確認する">
    <div class="deck-stack" style="gap: 0.6rem">
      <pre class="deck-code-panel" style="font-size: 1.14rem"><code>{{ log }}</code></pre>
      <div class="deck-check-grid">
        <div v-click class="deck-check-grid__item">HTTPメソッド<br />とパス</div>
        <div v-click class="deck-check-grid__item">ステータス<br />コード</div>
        <div v-click class="deck-check-grid__item">例外・<br />バリデーションエラー</div>
      </div>
      <p class="deck-note">問題を再現してから、同じ時刻のログを探す</p>
    </div>
  </DeckSlide>
</template>

<style scoped>
:deep(.slide-15 .deck-description__title) {
  font-size: 2.4rem;
}

:deep(.slide-15 .deck-description__body) {
  margin-top: 1rem;
}
</style>
