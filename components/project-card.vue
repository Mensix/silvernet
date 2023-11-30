<script setup lang="ts">
defineProps<{
  title: string
  description: string
  reverse?: boolean
}>()
</script>

<template>
  <section :class="!reverse && 'bg-zinc-900 border-y-2 border-zinc-800'">
    <div class="flex flex-col items-center justify-center gap-y-10 px-4 py-12 sm:px-12 lg:mx-auto lg:h-[75vh] lg:max-w-screen-lg lg:py-[24rem]">
      <div class="relative flex w-full flex-col items-center justify-center lg:justify-between lg:gap-32" :class="[reverse ? 'lg:flex-row-reverse' : 'lg:flex-row']">
        <div class="relative flex items-center justify-center lg:mb-0 lg:h-[400%]">
          <img src="/bubble1.svg" class="h-2/3 w-2/3 lg:h-full lg:w-full">
          <img src="/device1.png" class="absolute w-2/3 lg:w-1/2">
        </div>
        <div class="flex flex-col justify-center text-center lg:justify-start lg:text-left">
          <p class="text-lg font-medium text-red-400">
            Nasz projekt
          </p>
          <h2 class="relative mb-5 text-4xl font-extrabold text-zinc-100 underline decoration-red-400/25 decoration-[1rem] underline-offset-[-0.5rem] lg:text-5xl" style="text-decoration-skip-ink: none;">
            {{ title }}
          </h2>
          <p class="mb-5 leading-normal text-zinc-100 sm:[text-wrap:balance]  ">
            {{ description }}
          </p>
          <div class="flex flex-wrap justify-center gap-2 lg:justify-start">
            <app-store-button />
            <play-store-button />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
