<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="border-b border-slate-200">
    <nav class="mx-auto flex max-w-3xl items-center gap-6 p-4">
      <span class="font-semibold">Digital Diary</span>
      <RouterLink to="/" class="text-slate-600 hover:text-slate-900" active-class="text-slate-900">
        Home
      </RouterLink>
      <RouterLink
        to="/about"
        class="text-slate-600 hover:text-slate-900"
        active-class="text-slate-900"
      >
        About
      </RouterLink>
    </nav>
  </header>

  <main class="mx-auto max-w-3xl p-4">
    <RouterView />
  </main>
</template>
