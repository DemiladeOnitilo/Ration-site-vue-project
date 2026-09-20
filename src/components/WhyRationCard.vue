<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    cardItems: Object,
})

</script>

<template> 
    <div class="w-85 flex flex-col gap-2 border border-gray-300 rounded p-4">
        <div class="w-fit bg-cyan-500/30 rounded p-2">
            <component :is="cardItems.img" class="text-[#069]" :size="24" />
        </div>
        <h3 class="font-semibold text-lg">{{ cardItems.title }}</h3>
        <p class="text-md">{{ cardItems.description }}</p>
    </div>
</template>