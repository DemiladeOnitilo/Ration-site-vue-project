<script setup>
import FAQCards from "@/components/FAQCards.vue";
import faqs from "@/faq.json";
</script>

<template>
  <div
    class="bg-white flex items-center justify-center px-6 py-16 lg:px-0 lg:py-24"
  >
    <div
      class="max-w-2xl lg:max-w-5xl flex flex-col items-center justify-center gap-8"
    >
      <h1
        class="max-w-xl text-3xl md:text-4xl lg:text-5xl font-bold tracking-tight text-center"
      >
        Frequently Asked Questions
      </h1>
      <div class="w-full flex flex-col">
        <FAQCards v-for="faq in faqs.faqs" :key="faq.id" :faq="faq" />
      </div>
    </div>
  </div>
</template>
