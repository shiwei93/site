<script setup lang="ts">
import site from '@/data/site.config.json'
import DevIcon from '@/components/DevIcon.vue'

const fullYear = new Date().getFullYear()
</script>

<template>
  <footer>
    <div
      class="mt-16 mb-8 items-center justify-between space-y-3 md:flex md:space-y-0 text-sm text-gray-500 dark:text-gray-400"
    >
      <div class="flex items-center space-x-1">
        <span> Build with </span>
        <DevIcon category="IconVue" />
        <DevIcon category="IconTypescript" />
        <DevIcon category="IconTailwindcssVue" />
      </div>
      <div class="">
        © {{ fullYear }} {{ site.footerTitle }}
        <a href="https://beian.miit.gov.cn">苏ICP备2022046664号</a>
      </div>
    </div>
  </footer>
</template>
