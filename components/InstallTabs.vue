<script setup lang="ts">
import { computed, ref } from "vue";

import CommandBlock from "./CommandBlock.vue";

const options = [
  { id: "npm", label: "npm", command: "npm i" },
  { id: "pnpm", label: "pnpm", command: "pnpm i" },
  { id: "viteplus", label: "Vite+", command: "vp i" },
] as const;

const selected = ref<(typeof options)[number]["id"]>("viteplus");
const current = computed(() => options.find((option) => option.id === selected.value) ?? options[2]);

function select(id: (typeof options)[number]["id"]) {
  selected.value = id;
}

function move(offset: number) {
  const index = options.findIndex((option) => option.id === selected.value);
  const next = (index + offset + options.length) % options.length;
  selected.value = options[next].id;
}
</script>

<template>
  <div class="deck-install">
    <div class="deck-install__tabs" role="tablist" aria-label="パッケージマネージャー">
      <button
        v-for="option in options"
        :id="`tab-${option.id}`"
        :key="option.id"
        class="deck-install__tab"
        type="button"
        role="tab"
        :aria-controls="`panel-${option.id}`"
        :aria-selected="selected === option.id"
        :tabindex="selected === option.id ? 0 : -1"
        @click.stop="select(option.id)"
        @keydown.left.stop.prevent="move(-1)"
        @keydown.right.stop.prevent="move(1)"
      >
        {{ option.label }}
      </button>
    </div>
    <div
      :id="`panel-${current.id}`"
      class="deck-install__panel"
      role="tabpanel"
      :aria-labelledby="`tab-${current.id}`"
    >
      <CommandBlock :command="current.command" class="deck-command-card--wide" />
    </div>
  </div>
</template>
