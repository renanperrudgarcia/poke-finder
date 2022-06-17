<script setup>

const emit = defineEmits(['order-by'])
</script>

<template>
  <span class="mr-3">Ordenação:</span>
  <div class="inline-flex mb-8">
    <button
      class="bg-gray-300 hover:bg-gray-500 text-gray-800 font-bold py-2 px-3  rounded-1"
      @click="emit('order-by', 'id')"
    >
      1-9
    </button>
    <button
      class="border-l border-gray-200 bg-gray-300 hover:bg-gray-500 text-gray-800 font-bold py-2 px-3 rounded-r"
      @click="emit('order-by', 'name')"
    >
      A-Z
    </button>
  </div>
</template>
