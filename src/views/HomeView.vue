<script setup>
import HeroVue from '../components/layout/Hero.vue';
import CategoriesVue from '../components/homepage/Categories.vue';
import NewItemVue from '../components/homepage/NewItem.vue';
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
