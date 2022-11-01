<script setup>
import { RouterLink } from 'vue-router';

defineprops({
    title: String,
    count: Number,
    image: String,
})
</script>


<template>
    <div class="w-full px-1 my-1 md:w-1/2 lg:my-4 lg:px-4 lg:w-1/4">
        <div class="overflow-hidden border border-gray-200 rounded-xl">
            <Routerlink to="/">
                <div class="m-4 overflow-hidden rounded-xl">
                    <img :alt="title" class="block w-full h-auto" :src="image" />
                </div>
            </Routerlink>

            <header class="px-4 mb-4 leading-tight">
                <h1 class="text-lg">
                    <Routerlink class="font-semibold text-black no-underline hover:underline" to="/">
                        {{ title }}
                    </Routerlink>
                </h1>
                <span class="block text-sm font-light text-gray-500 no-underline">
                    {{ count }} items
                </span>
            </header>
        </div>
    </div>
</template>