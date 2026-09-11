<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="バグの調査方法 02">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title" style="font-size: 1.72rem">Consoleの赤いエラーから、失敗した場所を探す</h1>
        <ol class="deck-steps">
          <li v-click><span class="deck-steps__index">01</span><span>DevToolsを開く</span></li>
          <li v-click><span class="deck-steps__index">02</span><span>Consoleタブを選ぶ</span></li>
          <li v-click><span class="deck-steps__index">03</span><span>再現後、最初の赤いエラーを確認</span></li>
        </ol>
        <p class="deck-note" style="font-size: 1rem">エラーメッセージ・ファイル名・行番号を見る</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/16-chrome-devtools-console.jpg" alt="Chrome DevToolsのConsoleに表示されたエラー" />
      </figure>
    </div>
  </DeckSlide>
</template>
