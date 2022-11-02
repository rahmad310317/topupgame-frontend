<script setup>
import itemCard from '../landingPage/ItemCard.vue'
import { ref } from 'vue';

const newItem = ref([
    { id:1, title:'Mobile', image:'items-1.jpg' },
    { id:2, title:'Web Development', image:'items-2.jpg' },
    { id:3, title:'UI UX desaign', image:'items-3.jpg' }
])
</script>
<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
        <itemCard
        v-for="item in newItem" 
        :key="item.id"
        :title="item.title"
        :image="item.image" />
    </div>
</template>