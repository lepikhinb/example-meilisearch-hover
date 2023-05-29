<script setup lang="ts">
import BaseCard from "./BaseCard.vue";
</script>

<template>
  <BaseCard>
    <template #image>
      <img
        src="https://www.meilisearch.com/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fplug-n-play.9c2b8718.png&w=3840&q=100"
      />
    </template>

    <template #title> Plug ‘n play </template>

    <template #default>
      Deploy in a matter of minutes. Smart presets let you start searching
      through your data with zero configuration.
    </template>
  </BaseCard>
</template>
