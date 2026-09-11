<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRの作り方 03" title="PR作成画面を開く">
    <div class="deck-image-layout pr-entry-layout">
      <div class="deck-image-copy">
        <ol class="deck-steps">
          <li v-click><span class="deck-steps__index">01</span><span>GitHubでリポジトリを<br />開く</span></li>
          <li v-click><span class="deck-steps__index">02</span><span><strong>Compare &amp; pull request</strong>を選ぶ</span></li>
        </ol>
        <p class="deck-note">バナーがない場合は、ブランチ一覧から作業ブランチを開く</p>
      </div>

      <div class="pr-entry-visuals">
        <figure class="deck-image-frame deck-image-frame--banner pr-entry-visuals__banner">
          <img src="/images/11-compare-pull-request-banner.jpg" alt="GitHubに表示されたCompare & pull requestバナー" />
        </figure>
        <figure class="deck-image-frame pr-entry-visuals__branch">
          <img
            src="/images/11-branch-dropdown.jpg"
            alt="GitHubのブランチ一覧から作業ブランチを選ぶ画面"
            style="width: auto !important; height: 10.5rem !important; max-width: 100% !important"
          />
        </figure>
      </div>
    </div>
  </DeckSlide>
</template>

<style scoped>
.pr-entry-layout {
  grid-template-columns: minmax(17rem, 0.86fr) minmax(0, 1.5fr);
}

.pr-entry-visuals {
  display: grid;
  gap: 0.65rem;
  min-width: 0;
}

.pr-entry-visuals__banner {
  height: 4.5rem;
}

.pr-entry-visuals__branch {
  width: 16rem;
  height: 10.5rem;
  justify-self: end;
}

</style>
