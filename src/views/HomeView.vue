<script setup lang="ts">
import site from '@/data/site.config.json'
import Head from '@/components/Head.vue'
import ThemeSwitcher from '@/components/ThemeSwitcher.vue'
</script>

<template>
  <main>
    <Head :title="site.title" :description="site.description" />
    <h1 class="text-red-300 dark:text-red-100">Home</h1>
    <h2>This is subtitle</h2>
    <ThemeSwitcher />
  </main>
</template>
