<script setup>
import IncrementButton from '@/components/IncrementButton.vue'
import DecrementButton from '@/components/DecrementButton.vue'
import { ref } from 'vue'

const count = ref(0);
const increment = () => count.value++;
const decrement = () => {
	if(count.value > 0){
		count.value--;
	}
}


</script>

<template>
	<div class="flex items-center justify-center min-h-screen bg-gray-900">
    <div class="bg-gray-800 text-white rounded-lg p-4 max-w-xs flex flex-col items-center">
        <h3 class="text-lg font-semibold mb-4">Counter</h3>
        <div class="flex items-center space-x-4">
            <DecrementButton @decrement="decrement"/>
            <span class="text-2xl font-semibold">{{ count }}</span>
			<IncrementButton @increment="increment"/>
        </div>
    </div>
</div>
</template>