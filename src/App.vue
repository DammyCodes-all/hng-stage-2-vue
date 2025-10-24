<script setup lang="ts">
import { RouterView } from "vue-router";
import Footer from "./components/Footer.vue";
</script>

<template>
  <main class="max-w-[1440px] mx-auto min-h-dvh relative">
    <RouterView />
    <Footer />
  </main>
</template>
