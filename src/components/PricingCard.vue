<script setup>
import { Check, ExclamationCircle } from '@primeicons/vue';

 defineProps({
        price: Object
    })
</script>

<template>
    <div :class="[ price.id === '2' && 'border border-[#069] ', 'group w-[330px] min-h-[620px] bg-white text-black flex flex-col gap-6 p-6 rounded-xl shadow-xl hover:scale-[1.02] hover:border hover:border-[#069] transition-all duration-500 ease-in-out cursor-pointer']">
        <div class="flex flex-col gap-4">
            <p :class="[ price.id === '1' && 'text-black bg-gray-100', price.id === '2' && 'bg-[#069]/10 text-[#069]', price.id === '3' && 'bg-black text-white' , 'w-fit text-sm font-medium tracking-tight rounded-full px-3 py-0.5 uppercase']">{{ price.type }}</p>
            <h3 class="text-2xl font-semibold tracking-tight">{{ price.title }}</h3>
            <h2 class="text-3xl font-bold tracking-tight">{{ price.amount }} <span class="text-xl text-gray-400 font-light">/user /year</span></h2>
            <p class="text-md tracking-tight">Billed Annually</p>
        </div>
        <div class="flex flex-col gap-2">
            <p class="text-gray-500 text-sm tracking-tight">{{ price.subtext }}</p>
            <div class="flex flex-col gap-4">
                <div v-for="item in price.subtextList" :key="item" class="flex items-center gap-2">
                    <span class=" w-fit bg-[#069] text-white p-1 rounded-full">
                        <Check :size="15"/>
                    </span>
                    <p class="text-xs">{{ item }}</p>
                </div>  
            </div>
            
        </div>
        <ul v-if="price.extras" class="flex flex-col gap-2 list-disc pl-6">
            <li v-for="(extra, index) in price.extras" :key="index" class="text-sm text-gray-400">{{ extra }}</li>
        </ul>
        <div v-else-if="price.addOns" class="flex gap-2 bg-gray-100 p-2" >
            <span :class="[price.id === '2' ? 'bg-[#069] text-white' : 'text-gray-500 group-hover:bg-[#069] group-hover:text-white','h-fit rounded-full']">
                <ExclamationCircle :size="20"/>
            </span>
            <p class="text-xs">{{ price.addOns }}</p>
        </div>
        <button :class="[ price.id === '2' ? 'bg-[#069] hover:bg-cyan-600 text-white' : 'border border-gray-300 text-black group-hover:bg-[#069] hover:bg-cyan-600 group-hover:text-white'  ,  'w-full text-sm font-medium px-10 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer']">
            {{ price.button }}
        </button>
    </div>
</template>