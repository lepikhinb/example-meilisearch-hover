<script setup lang="ts">
import BaseCard from "./BaseCard.vue";
</script>

<template>
  <BaseCard>
    <template #image>
      <img
        src="https://www.meilisearch.com/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Ffast.cf656ef1.png&w=3840&q=100"
      />
    </template>

    <template #title> Lightning fast </template>

    <template #default>
      Search-as-you-type returns answers in less than 50 milliseconds. That's
      faster than the blink of an eye!
    </template>
  </BaseCard>
</template>
