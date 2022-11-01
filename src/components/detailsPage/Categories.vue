<script setup>
import CategoriesCardVue from '../landingPage/CategoriesCard.vue';
</script>
<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
        <CategoriesCardVue title="Mobile UI Kit" count="534" image="categories-1.jpg" />
        <CategoriesCardVue title="Fonts" count="675" image="categories-2.jpg" />
        <CategoriesCardVue title="Icons" count="431" image="categories-3.jpg" />
        <CategoriesCardVue title="Website Ui Kit" count="321" image="categories-4.jpg" />
    </div>


</template>