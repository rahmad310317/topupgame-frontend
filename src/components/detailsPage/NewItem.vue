<script setup>
import NewItemCardVue from '../landingPage/NewItemCard.vue';
</script>
<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
       <NewItemCardVue title="Mobile" image="items-1.jpg" />
       <NewItemCardVue title="Mobile" image="items-2.jpg" />
       <NewItemCardVue title="Mobile" image="items-3.jpg" />
    </div>
</template>