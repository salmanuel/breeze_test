<template>
  <div class="bg-gray-200 rounded-lg p-4 shadow-lg">
    <h2 class="text-xl font-bold mb-2">{{ item.name }}</h2>
    <p class="text-gray-600 mb-2">{{ item.description }}</p>
    <div class="flex justify-between">
      <p class="text-right">Quantity: {{ item.quantity }}</p>
      <p class="text-right">Price: ${{ item.price }}</p>
    </div>
  </div>
</template>

<script setup>

defineProps({
  item: Object,
});
</script>
