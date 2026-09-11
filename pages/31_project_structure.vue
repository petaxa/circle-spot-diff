<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";

const tree = `.
├── frontend/       Vue + Vue Router + Vize
├── backend/        Hono REST API
└── documentation/  Ox Contentのシステム仕様書`;
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 06" title="プロジェクトの構成">
    <div class="deck-stack">
      <pre class="deck-code-panel" style="font-size: 1.42rem"><code>{{ tree }}</code></pre>
      <p class="deck-note">画面の問題は <span class="deck-inline-code">frontend/</span>、APIの問題は <span class="deck-inline-code">backend/</span> から調べる</p>
    </div>
  </DeckSlide>
</template>
