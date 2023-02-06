// https://galpratama.notion.site/Handbook-Front-end-Developer-Mastering-Vue-JS-3-e7aa7200699f4647bf67d3d882ed1120
// https://zullkit-backend.demo.belajarkoding.com/ email: admin@email.co ps:password
<script setup>
import { RouterView } from "vue-router";
import Navbar from '@/components/layouts/Navbar.vue'
</script>

<template>
  <Navbar />
  <RouterView />
</template>

<style>
@import "@/assets/css/styles.css";
</style>
