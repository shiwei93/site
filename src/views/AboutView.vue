<script setup lang="ts">
import site from '@/data/site.config.json'
import Head from '@/components/Head.vue'
</script>

<template>
  <div class="about">
    <Head :title="`About - ${site.title}`" :description="site.description" />
    <h1>This is an about page</h1>
  </div>
</template>
