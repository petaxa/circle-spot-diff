<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="開発環境のセットアップ 01">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title">リポジトリをcloneする</h1>
        <CommandBlock command="git clone https://github.com/<owner>/<repository>.git" class="deck-command-card--compact" />
        <p class="deck-note">自分たちのリポジトリのCodeメニューからURLをコピーする</p>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/22-code-clone-url.jpg" alt="GitHubのCodeメニューに表示されたclone URL" />
      </figure>
    </div>
  </DeckSlide>
</template>
