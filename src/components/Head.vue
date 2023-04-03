<script setup lang="ts">
import { Head } from '@vueuse/head'

const props = defineProps<{
  title: string
  description: string
}>()
</script>

<template>
  <Head>
    <title>{{ props.title }}</title>
    <mete name="description">{{ props.description }}</mete>
  </Head>
</template>
