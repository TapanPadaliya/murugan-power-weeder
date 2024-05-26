<template>
  <header class="flex items-center justify-between py-2">
    <div><img src="/full-logo.png" class="max-h-8" /></div>
    <div class="flex gap-3">
      <nuxt-link
        v-for="(item, i) in allRoutes"
        :key="i"
        :to="item.path"
        class="hover:underline"
      >
        {{ item.name }}
      </nuxt-link>
    </div>
  </header>
</template>
<script setup lang="ts">
const allRoutes = [
  { path: "/", name: "Home" },
  { path: "/weeders", name: "Weeders" },
  { path: "/about", name: "About" },
];
</script>
