<script setup lang="ts">
import { useHead } from '@vueuse/head'

useHead({
  title: 'Home',
  meta: [
    {
      name: 'description',
      content: 'This is the home page'
    }
  ]
})
</script>

<template>
  <main>
    <h1 class="text-red-300">Home</h1>
    <h2>This is subtitle</h2>
  </main>
</template>
