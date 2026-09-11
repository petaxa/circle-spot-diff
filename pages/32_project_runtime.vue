<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 07" title="起動先とデータの扱い">
    <div class="deck-stack">
      <div class="deck-url-list">
        <div class="deck-url-list__row"><span class="deck-url-list__label">フロントエンド</span><span class="deck-url-list__value">http://127.0.0.1:5173</span></div>
        <div class="deck-url-list__row"><span class="deck-url-list__label">バックエンド</span><span class="deck-url-list__value">http://127.0.0.1:8787</span></div>
        <div class="deck-url-list__row"><span class="deck-url-list__label">ヘルスチェック</span><span class="deck-url-list__value">http://127.0.0.1:8787/api/health</span></div>
        <div class="deck-url-list__row"><span class="deck-url-list__label">システム仕様書</span><span class="deck-url-list__value">http://127.0.0.1:4174</span></div>
      </div>
      <p v-click class="deck-callout" style="font-size: 1.5rem">APIのデータはインメモリ。<br />バックエンドを再起動すると初期状態に戻る</p>
    </div>
  </DeckSlide>
</template>
