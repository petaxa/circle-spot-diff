<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";

const commands = `vp run dev:all     # フロントエンドとバックエンドを起動
vp run build:all   # アプリと仕様書をビルド
vp run docs:dev    # システム仕様書を起動
vp run docs:build  # システム仕様書をビルド`;
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 04" title="開発で使う主なコマンド">
    <pre class="deck-code-panel" style="font-size: 1.42rem"><code>{{ commands }}</code></pre>
  </DeckSlide>
</template>
