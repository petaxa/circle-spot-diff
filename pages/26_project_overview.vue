<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 01">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title" style="font-size: 2.35rem">Tasklyは、毎日のタスクを管理するToDoアプリ</h1>
        <dl class="deck-term-list">
          <div v-click class="deck-term-list__row">
            <dt>Frontend</dt><dd>Vue + Vue Router + Vize</dd>
          </div>
          <div v-click class="deck-term-list__row">
            <dt>Backend</dt><dd>Hono REST API</dd>
          </div>
        </dl>
        <p class="deck-note" style="font-size: 1rem">フロントエンドとバックエンドは、独立したViteアプリ</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/26-taskly-overview.jpg" alt="Tasklyの概要画面" />
      </figure>
    </div>
  </DeckSlide>
</template>
