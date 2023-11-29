<script setup lang="ts">
useHead({
  bodyAttrs: {
    class: 'bg-zinc-950 font-[\'Open_Sans\']',
  },
})
</script>

<template>
  <navbar />
  <hero />
  <project-card title="Plan WZIM" description="Plan WZIM to aplikacja służąca do sprawdzania planu zajęć studentów i prowadzących na Wydziale Zastosowań Informatyki i Matematyki." />
  <project-card title="Kampus SGGW" description="Aplikacja powstała, aby pomóc osobom przebywającym na kampusie Szkoły Głównej Gospodarstwa Wiejskiego w odnalezieniu budynków oraz innych znaczących lokalizacji." reverse />
  <plans />
  <join />
  <foot />
</template>
