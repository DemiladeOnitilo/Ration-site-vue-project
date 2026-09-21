<script setup>

defineProps({
    cardItems: Object,
})

</script>

<template> 
    <div class="w-85 flex flex-col gap-2 border border-gray-200 rounded-xl p-4">
        <div class="w-fit bg-[#069]/20 rounded p-2">
            <component :is="cardItems.img" class="text-[#069]" :size="24" />
        </div>
        <h3 class="font-semibold text-lg">{{ cardItems.title }}</h3>
        <p class="text-md">{{ cardItems.description }}</p>
    </div>
</template>