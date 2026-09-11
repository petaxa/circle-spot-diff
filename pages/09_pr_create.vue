<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="PRの作り方 04" title="Descriptionを書いて作成する">
    <div class="deck-image-layout pr-create-layout">
      <div class="deck-image-copy">
        <ol class="deck-steps">
          <li v-click>
            <span class="deck-steps__index">01</span>
            <span>baseは <span class="deck-inline-code">main</span><br />compareは作業ブランチ</span>
          </li>
          <li v-click>
            <span class="deck-steps__index">02</span>
            <span>TitleとDescriptionへ<br />修正内容と確認方法を書く</span>
          </li>
          <li v-click>
            <span class="deck-steps__index">03</span>
            <span><strong>Create pull request</strong>を選ぶ</span>
          </li>
        </ol>
      </div>

      <figure class="deck-image-frame pr-create-screen">
        <img
          src="/images/09-create-pull-request-form.png"
          alt="GitHubのPull Request作成フォーム。Title、Description、Create pull requestボタンが表示されている"
          style="width: auto !important; height: 18rem !important; max-width: 100% !important"
        />
      </figure>
    </div>
  </DeckSlide>
</template>

<style scoped>
.pr-create-layout {
  grid-template-columns: minmax(18rem, 0.82fr) minmax(0, 1.18fr);
  gap: 2rem;
}

.pr-create-screen {
  height: 18rem;
  background: var(--deck-code-bg);
}

</style>
