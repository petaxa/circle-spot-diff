<script setup lang="ts">
import CommandBlock from "../components/CommandBlock.vue";
import DeckSlide from "../components/DeckSlide.vue";

const command = `git add <変更したファイル>
git commit -m "fix: <直した内容>"
git push -u origin fix/<短い名前>`;
</script>

<template>
  <DeckSlide section-label="PRの作り方 02" title="変更をコミットしてPushする">
    <div class="deck-command-stack">
      <CommandBlock :command="command" class="deck-command-card--wide deck-command-card--compact" />
      <p class="deck-note">最初のPushでは <span class="deck-inline-code">-u</span> で追跡先を設定する</p>
    </div>
  </DeckSlide>
</template>
