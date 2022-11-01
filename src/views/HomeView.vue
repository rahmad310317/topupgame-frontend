<script setup>
import HeroVue from '../components/landingPage/Hero.vue';
import CategoriesVue from '../components/homePage/Categories.vue';
import NewItemVue from '../components/homePage/NewItem.vue';
</script>

<template>
  <main>
    <HeroVue />
    
    <div class="container px-4 mx-auto my-16 md:px-12">
      <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
      <CategoriesVue />
    </div>

    <div class="container px-4 mx-auto my-16 md:px-12">
      <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
      <NewItemVue />
    </div>
  </main>
</template>
