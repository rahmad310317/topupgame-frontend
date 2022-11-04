<script setup>

import DescriptionVue from '../components/productpage/Description.vue';
import GalleryVue from '../components/productpage/Gallery.vue';
import Complate from '../components/productpage/Complate.vue';
</script>

<template>
    <main>
        <div class="conztainer p-2 mx-auto my-10 max-w-7xl">
            <div class="flex flex-row flex-wrap py-4">
                <main role="main" class="w-full px-4 pt-1 sm:w-2/3 md:w-2/3">
                    <h1
                        class="mb-2 text-3xl font-bold leading-normal tracking-tight text-gray-900 sm:text-4xl md:text-4xl">
                        RoboCrypto UI Kit
                    </h1>
                    <p class="text-gray-500">Build your next coin startup</p>
                    <!-- gallery -->
                    <GalleryVue />
                    <section class="" id="orders">
                        <h1 class="mt-8 mb-3 text-lg font-semibold">About</h1>
                        <!-- about -->
                        <DescriptionVue />
                    </section>
                </main>
                <aside class="w-full px-4 sm:w-1/3 md:w-1/3">
                    <!-- complate item-->
                    <Complate />
                </aside>
            </div>
        </div>
    </main>
</template>