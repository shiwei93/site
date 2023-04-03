<script setup lang="ts">
import { RouterLink } from 'vue-router'
import ThemeSwitcher from '@/components/ThemeSwitcher.vue'
import MoreNav from '@/components/MoreNav.vue'
import { navigationLinks } from '@/data/navigationLinks'
</script>

<template>
  <header class="sticky top-0 backdrop-blur">
    <div class="flex items-center z-40 py-4 lg:px-8 lg:mx-0 mx-4">
      <RouterLink to="/">
        <img src="@/assets/images/logo.png" alt="logo" class="h-12 w-12 mr-2 rounded-full" />
      </RouterLink>
      <div class="ml-auto flex items-center">
        <nav class="hidden text-base leading-6 font-semibold space-x-5 md:flex">
          <RouterLink
            v-for="{ to, title } in navigationLinks"
            :key="title"
            class="text-slate-700 dark:text-slate-300 opacity-70 hover:opacity-100 transition-opacity"
            :to="to"
          >
            {{ title }}
          </RouterLink>
        </nav>
        <div
          class="flex items-center border-l-0 border-slate-200 md:border-l ml-6 pl-5 dark:border-slate-800"
        >
          <ThemeSwitcher />
          <MoreNav />
        </div>
      </div>
    </div>
  </header>
</template>
