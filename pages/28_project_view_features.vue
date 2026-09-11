<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 03">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title">タスクの見方</h1>
        <ol class="deck-steps">
          <li><span class="deck-steps__index">01</span><span>タスクリスト</span></li>
          <li v-click="1"><span class="deck-steps__index">02</span><span>ガントチャート</span></li>
          <li v-click="2"><span class="deck-steps__index">03</span><span>バーンダウンチャート</span></li>
          <li v-click="3"><span class="deck-steps__index">04</span><span>集計</span></li>
          <li v-click="4"><span class="deck-steps__index">05</span><span>絞り込み</span></li>
        </ol>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <div class="deck-image-swap">
          <img v-click.hide="1" src="/images/28-taskly-list.png" alt="Tasklyのタスクリスト" />
          <div v-click="1" class="deck-image-stage">
            <img v-click.hide="2" src="/images/28-taskly-gantt-new.png" alt="Tasklyのガントチャート" />
          </div>
          <div v-click="2" class="deck-image-stage">
            <img v-click.hide="3" src="/images/28-taskly-burndown-new.png" alt="Tasklyのバーンダウンチャート" />
          </div>
          <div v-click="3" class="deck-image-stage">
            <img v-click.hide="4" src="/images/28-taskly-summary-crop.png" alt="Tasklyの進捗と期限の集計" />
          </div>
          <div v-click="4" class="deck-image-stage">
            <img src="/images/28-taskly-filter.png" alt="Tasklyのキーワードと完了状態による絞り込み" />
          </div>
        </div>
      </figure>
    </div>
  </DeckSlide>
</template>

<style scoped>
.deck-image-stage {
  position: absolute;
  inset: 0;
  display: grid;
  width: 100%;
  height: 100%;
  place-items: center;
}

.deck-image-stage img {
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.deck-image-copy .deck-steps li {
  padding: 0.46rem 0;
  font-size: 1rem;
  white-space: nowrap;
}
</style>
