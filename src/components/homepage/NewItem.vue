<script setup>
import itemCard from '../layout/ItemCard.vue';
import axios from 'axios';
import { ref, onMounted} from 'vue';

const newItems = ref([]);
async function getnewitem(){
    try {
        const respone = await axios.get('http://zullkit-backend.buildwithangga.id/api/products');
        newItems.value = respone.data.data.data;        
    } catch (error) {
        console.log(error);
    }
}

onMounted(() => {
    getnewitem();
});
 
</script>

<template>
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
        <itemCard
        v-for="item in newItems" 
        :key="item.id"
        :id="item.id"
        :description="item.subtitle"
        :title="item.name"
        :image="item.thumbnails"
            
        />
    </div>
</template>