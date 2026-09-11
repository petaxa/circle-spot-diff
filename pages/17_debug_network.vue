<script setup lang="ts">
import DeckSlide from "../components/DeckSlide.vue";
</script>

<template>
  <DeckSlide section-label="バグの調査方法 03">
    <div class="deck-image-layout">
      <div class="deck-image-copy">
        <h1 class="deck-body-title" style="font-size: 2.05rem">Networkで、送信内容とAPIの返答を確認する</h1>
        <ol class="deck-steps">
          <li><span class="deck-steps__index">01</span><span>Networkを開き、Fetch/XHRに絞る</span></li>
          <li><span class="deck-steps__index">02</span><span>問題を再現して通信を選ぶ</span></li>
          <li><span class="deck-steps__index">03</span><span>Request・Status・Responseを見る</span></li>
        </ol>
      </div>
      <figure class="deck-image-frame deck-image-frame--tall">
        <div class="deck-image-swap">
          <img v-click.hide="1" src="/images/17-chrome-devtools-network.jpg" alt="Chrome DevToolsのNetwork一覧" />
          <img v-click="1" src="/images/17-chrome-devtools-response.jpg" alt="Chrome DevToolsのNetwork Responseタブ" />
        </div>
        <div v-click.hide="1" class="deck-image-labels">
          <span class="deck-image-label">REQUEST</span>
          <span class="deck-image-label">STATUS</span>
        </div>
        <div v-click="1" class="deck-image-labels"><span class="deck-image-label">RESPONSE</span></div>
        <p v-click="2" class="deck-image-overlay-note">通信が見つからない場合は、フロントエンド側で処理が止まっている可能性がある</p>
      </figure>
    </div>
  </DeckSlide>
</template>
