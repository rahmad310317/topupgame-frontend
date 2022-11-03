<script setup>
import { ref } from 'vue';
import CategoriesCardVue  from '../layout/CategoriesCard.vue';


const categories = ref([
    { id: 1, title: 'Mobile Ui Kit', count: 534, image: 'categories-1.jpg' },
    { id: 2, title: 'Fonts', count: 657, image: 'categories-2.jpg' },
    { id: 3, title: 'Icons', count: 431, image: 'categories-3.jpg' },
    { id: 4, title: 'Website Ui Kit', count: 321, image: 'categories-4.jpg' }

])
</script>

<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
        <CategoriesCardVue 
         v-for=" category in categories " 
        :key="category.id"
        :title="category.title"
        :count="category.count"
        :image="category.image" />
    </div>

</template>