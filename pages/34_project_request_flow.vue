<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 09" title="画面操作からAPI応答までの流れ">
    <div class="deck-stack" style="gap: 1rem">
      <div class="deck-flow">
        <div v-click class="deck-flow__item"><span class="deck-flow__index">01</span><p class="deck-flow__text"><span class="deck-inline-code">views/</span>が操作を受け取る</p></div>
        <div v-click class="deck-flow__item"><span class="deck-flow__index">02</span><p class="deck-flow__text"><span class="deck-inline-code">api/todos.ts</span>を呼ぶ</p></div>
        <div v-click class="deck-flow__item"><span class="deck-flow__index">03</span><p class="deck-flow__text">ブラウザが<span class="deck-inline-code">:8787/api</span>へ送信</p></div>
        <div v-click class="deck-flow__item"><span class="deck-flow__index">04</span><p class="deck-flow__text"><span class="deck-inline-code">backend/src/index.ts</span>のHonoルート</p></div>
        <div v-click class="deck-flow__item"><span class="deck-flow__index">05</span><p class="deck-flow__text">インメモリを読み書きしJSONを返す</p></div>
        <div v-click class="deck-flow__item"><span class="deck-flow__index">06</span><p class="deck-flow__text">画面がレスポンスを反映する</p></div>
      </div>
      <p v-click class="deck-note">止まった段階に合わせて、Console、Network、バックエンドログを確認する</p>
    </div>
  </DeckSlide>
</template>
