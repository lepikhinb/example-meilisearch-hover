<script setup lang="ts">
import BaseCard from "./BaseCard.vue";
</script>

<template>
  <BaseCard>
    <template #image>
      <img
        src="https://www.meilisearch.com/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Frelevant.f3662a46.png&w=3840&q=100"
      />
    </template>

    <template #title> Ultra relevant </template>

    <template #default>
      Take advantage of the most advanced full-text search engine with its
      out-of-the-box great relevancy that fits every use case.
    </template>
  </BaseCard>
</template>
