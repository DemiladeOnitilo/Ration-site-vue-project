<script setup>
import { Minus, Plus } from '@primeicons/vue';
import { ref } from 'vue';

 defineProps({
    faq: Object,
})

const isVisible = ref(false)

</script>

<template>
    <div :class="[ isVisible ? 'bg-gray-100' : 'bg-white' ,'w-[1000px] flex items-center justify-between p-4 border-b border-gray-200 transition-all duration-500 ease-in-out']">
        <div class="flex flex-col gap-4">
            <h3 :class="[ isVisible ? 'text-[#069]' : 'text-black' , 'text-lg font-semibold transition-colors duration-500 ease-in-out']">{{ faq.title }}</h3>
            <div v-show="isVisible" :class="[ isVisible ? 'max-h-40 opacity-100 mt-2' : 'max-h-0 opacity-0 mt-0', 'text-sm text-gray-600 transition-all duration-500 ease-in-out overflow-hidden']">
                <p>{{ faq.subText }}</p>
            </div>
        </div>
        <div @click="isVisible = !isVisible" :class="[ isVisible ? 'bg-[#069] text-white border-[#069]' : 'hover:bg-[#069] border-black text-black', 'h-fit flex items-center justify-center rounded-full border p-0.5 cursor-pointer transition-all duration-500 ease-in-out']">
            <Minus v-if="isVisible" :size="15"/>
            <Plus v-else :size="15" />
        </div>
    </div>
</template>