<script setup lang="ts">
import IconVue from '@/components/icons/IconVue.vue'
import IconTypescript from '@/components/icons/IconTypescript.vue'
import IconTailwindcssVue from '@/components/icons/IconTailwindcss.vue'

const DevIconsMap = {
  IconVue,
  IconTypescript,
  IconTailwindcssVue
}
type Category = keyof typeof DevIconsMap

const Links = {
  IconVue: 'https://vuejs.org/',
  IconTypescript: 'https://www.typescriptlang.org/',
  IconTailwindcssVue: 'https://tailwindcss.com/'
}

const { category } = defineProps<{
  category: Category
}>()
const Icon = DevIconsMap[category]
const link = Links[category]
</script>

<template>
  <a :href="link"><Icon class="h-5 w-5" /></a>
</template>
