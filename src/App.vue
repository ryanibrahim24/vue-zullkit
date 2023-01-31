// https://galpratama.notion.site/Bootcamp-VueJS-3-Handbook-e7aa7200699f4647bf67d3d882ed1120
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
