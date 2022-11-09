<script setup>
import { ref, onMounted } from 'vue';
import axios from 'axios';

import CategoriesCardVue from '../layout/CategoriesCard.vue';


const categories = ref([]);

// function api data tanpa promise
async function getCategoriesData() {
    try {
        const respone = await axios.get('http://zullkit-backend.buildwithangga.id/api/categories');
        categories.value  = respone.data.data.data;
    } catch (error) {
        console.log(error);
    }
   
}
// mounted data
onMounted(() => {
    getCategoriesData();
});

</script>

<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg" id="categories">All Categories</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
        <CategoriesCardVue 
            v-for="category in categories"
            :key="category.id"
            :id="category.id"
            :title="category.name"
            :count="category.count"
            :image="category.thumbnails"
        />
    </div>
</template>