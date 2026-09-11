<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="デモプロジェクトの基礎知識 02">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title">タスクに対する操作</h1>
        <dl class="deck-term-list">
          <div v-click class="deck-term-list__row"><dt>追加</dt><dd>開始日と期限を含むタスクを登録</dd></div>
          <div v-click class="deck-term-list__row"><dt>更新</dt><dd>タスク名と完了状態を変更</dd></div>
          <div v-click class="deck-term-list__row"><dt>削除</dt><dd>不要なタスクを削除</dd></div>
          <div v-click class="deck-term-list__row"><dt>詳細</dt><dd>一件のタスク情報を表示</dd></div>
        </dl>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <img src="/images/27-taskly-task-list.jpg" alt="Tasklyのタスクリスト画面" />
      </figure>
    </div>
  </DeckSlide>
</template>
