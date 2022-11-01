<script setup>
import HeroVue from '../components/landingPage/Hero.vue';
import CategoriesVue from '../components/detailsPage/Categories.vue';
import NewItemVue from '../components/detailsPage/NewItem.vue';
</script>

<template>
  <main>
    <HeroVue />
    <div class="container px-4 mx-auto my-16 md:px-12">    
      <CategoriesVue/>
    </div>
    <div class="container px-4 mx-auto my-16 md:px-12">    
      <NewItemVue />
    </div>
  </main>
</template>
