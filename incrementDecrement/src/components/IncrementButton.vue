<script setup>
const emit = defineEmits(['increment'])
</script>

<template>
	<button @click="$emit('increment')" class="bg-gray-700 hover:bg-gray-600 text-white font-bold py-2 px-4 rounded">+</button>
</template>