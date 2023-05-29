<script setup lang="ts">
import { ref } from "vue";
import { useMouseInElement } from "@vueuse/core";

const card = ref<HTMLDivElement>();
const { elementX, elementY } = useMouseInElement(card);
</script>

<template>
  <div
    ref="card"
    :style="{
      '--x': `${elementX}px`,
      '--y': `${elementY}px`,
    }"
    class="border-gradient group relative before:blur-xl overflow-hidden border border-b-0 border-white/5 rounded-2xl bg-[#201E22] p-4 before:absolute before:-inset-px before:h-[calc(100%+2px)] before:w-[calc(100%+2px)] before:rounded-xl lg:p-8"
  >
    <div class="relative">
      <div class="">
        <slot name="image" />
      </div>

      <div class="mt-5 text-2xl font-medium text-white">
        <slot name="title" />
      </div>

      <div class="mt-3 text-sm font-light text-white/60">
        <slot />
      </div>
    </div>
  </div>
</template>

<style>
.border-gradient::before {
  background: radial-gradient(
    350px circle at var(--x) var(--y),
    #663dc770 0%,
    transparent 100%
  );
}
</style>
