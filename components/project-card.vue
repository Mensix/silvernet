<script setup lang="ts">
defineProps<{
  title: string
  description: string
}>()
</script>

<template>
  <section class="flex flex-col items-center justify-center px-4 py-12">
    <div class="relative flex w-full flex-col items-center justify-center">
      <div class="relative mb-10 flex items-center justify-center">
        <img src="/bubble1.svg" class="h-full w-full">
        <img src="device1.png" class="absolute w-5/6">
      </div>
      <p class="text-lg font-medium text-red-400">
        Nasz projekt
      </p>
      <h2 class="relative mb-5 text-4xl font-extrabold text-zinc-100 underline decoration-red-400/25 decoration-[1rem] underline-offset-[-0.5rem]" style="text-decoration-skip-ink: none;">
        {{ title }}
      </h2>
      <p class="mb-5 text-center leading-normal text-zinc-100">
        {{ description }}
      </p>
      <div class="flex flex-wrap justify-center gap-2">
        <app-store-button />
        <play-store-button />
      </div>
    </div>
  </section>
</template>
