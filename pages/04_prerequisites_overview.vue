<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="前提知識" title="このあと説明すること">
    <ol class="deck-recap">
      <li v-click>
        <span class="deck-recap__index">01</span>
        <span class="deck-recap__keyword">PR</span>
        <span class="deck-recap__text">修正を共有し、レビューを経て取り込むまで</span>
      </li>
      <li v-click>
        <span class="deck-recap__index">02</span>
        <span class="deck-recap__keyword">調査</span>
        <span class="deck-recap__text">ログ、コンソール、通信履歴から原因を絞る</span>
      </li>
    </ol>
  </DeckSlide>
</template>
