<script setup>
const emit = defineEmits(['decrement'])
</script>

<template>
	<button @click="$emit('decrement')" class="bg-gray-700 hover:bg-gray-600 text-white font-bold py-2 px-4 rounded">-</button>
</template>