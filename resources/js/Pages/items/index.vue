<template>
    <div class="bg-white  overflow-hidden ml-2 mr-2">
        <div class="flex justify-between mt-2 mb-2">
            <h1 class="ml-2 text-4xl font-bold"><i class="fa-solid fa-book-bookmark"></i>items</h1>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 p-4 ">
            <ItemCard v-for="item in items" :key="item.id" :item="item" />
            <!-- <div v-for="item in items" :key="item.id" class="bg-gray-200 rounded-lg p-4 shadow-lg">
                <h2 class="text-xl font-bold mb-2">{{ item.name }}</h2>
                <p class="text-gray-600 mb-2">{{ item.description }}</p>
                <div class="flex justify-between">
                    <p class="text-right">Quantity: {{ item.quantity }}</p>
                    <p class="text-right">Price: ${{ item.price }}</p>
                </div>
            </div> -->
        </div>
    </div>
</template>

<script setup>
import ItemCard from '../../Components/ItemCard.vue'

defineProps({
    items: Array,
});
</script>
