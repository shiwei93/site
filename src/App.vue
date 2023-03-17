<script setup lang="ts">
import { RouterView } from 'vue-router'
import Navigation from '@/components/Navigation.vue'
import Footer from '@/components/Footer.vue'
</script>

<template>
  <Navigation />
  <section class="mx-auto max-w-3xl px-3 sm:px-6 xl:max-w-5xl xl:px-0">
    <RouterView />
    <Footer />
  </section>
</template>
