<script setup>
import FAQCards from '@/components/FAQCards.vue';
import faqs from '@/faq.json'

</script>

<template>
    <div class="bg-white flex items-center justify-center">
        <div class="max-w-[100px] lg:max-w-5xl flex flex-col items-center justify-center gap-8 py-24">
            <h1 class="text-5xl font-bold tracking-tight">Frequently Asked Questions</h1>
            <div class="w-full flex flex-col">
                <FAQCards v-for="faq in faqs.faqs" :key="faq.id" :faq="faq" />
            </div>
        </div>   
    </div>
    
</template>