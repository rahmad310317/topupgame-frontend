<script setup>
import {RouterView} from 'vue-router';
import NavbarVue from './components/homepage/Navbar.vue';
</script>

<template>
  <NavbarVue />
  <RouterView />
</template>

<style>
@import '@/assets/css/styles.css';
</style>
