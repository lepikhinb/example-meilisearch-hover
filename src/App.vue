<script setup lang="ts">
import FastCard from "./components/FastCard.vue";
import PlugCard from "./components/PlugCard.vue";
import UltraCard from "./components/UltraCard.vue";
</script>

<template>
  <div
    class="relative flex h-screen w-screen items-center justify-center bg-[#18181b] p-16"
  >
    <div class="max-w-5xl w-full">
      <div class="mx-auto text-center">
        <h1 class="text-5xl font-semibold text-white">
          The next generation of search
        </h1>

        <p class="mt-5 text-lg text-white/90">
          Meilisearch is a flexible and powerful user-focused search engine
          <br />
          that can be added to any website or application.
        </p>
      </div>

      <div class="mt-12 grid grid-cols-3 gap-8">
        <FastCard />

        <PlugCard />

        <UltraCard />
      </div>
    </div>
  </div>
</template>
