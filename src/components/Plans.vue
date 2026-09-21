<script setup>
import { Check } from '@primeicons/vue';

defineProps({
        plans: Object
    })
</script>

<template>
    <div class="w-[330px] h-[420px] bg-white text-black flex flex-col justify-between  p-6 rounded-xl shadow-xl">
        <div class="w-full flex flex-col items-center justify-center gap-2 text-center">
            <h3 class="w-full max-w-[160px] text-sm font-semibold tracking-tight">{{ plans.title }}</h3>
            <p class="text-xs text-gray-500 tracking-tight">{{ plans.subtext}}</p>
        </div>
        <div class="flex flex-col gap-4 mt-2">
            <div v-for="(item, index) in plans.subtextList" :key="index" class="flex items-center gap-2">
                <span class=" w-fit bg-[#069] text-white p-1 rounded-full">
                    <Check :size="15"/>
                </span>
                <p class="text-xs">{{ item }}</p>
            </div>  
        </div> 
        <button class="bg-[#069] hover:bg-cyan-600 w-full text-sm text-white font-medium px-10 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer">
            Get Started
        </button>
    </div>
</template>