<script setup lang="ts">
defineProps<{
  title: string
  description?: string
}>()
</script>

<template>
  <div class="rounded-3xl border-2 border-zinc-800 bg-zinc-900 p-6">
    <h3 class="mb-5 text-3xl font-extrabold text-red-400">
      {{ title }}
    </h3>
    <p class="leading-normal text-zinc-100">
      {{ description }}
      <slot v-if="!description" name="description" />
    </p>
  </div>
</template>
