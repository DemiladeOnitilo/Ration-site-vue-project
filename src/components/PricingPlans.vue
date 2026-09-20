<script setup>
import PricingCard from './PricingCard.vue';
import pricing from "@/pricing.json"

</script>

<template>
  <div
    class="bg-gray-100 flex flex-col items-center justify-center gap-8 py-24"
  >
    <div class="flex flex-col justify-center items-center gap-2">
      <h1 class="text-5xl font-bold tracking-tight">Pricing Plans</h1>
      <p class="font-medium">
        Start with collaboration. Do the work. Scale with confidence.
      </p>
      <div class="flex items-center gap-2">
        <p class="text-sm text-gray-500">Select your currency:</p>
        <select
          name="currency"
          id=""
          class="bg-gray-200 border border-gray-500 hover:bg-gray-400 px-2 py-1 transition-all duration-300 ease-in-out cursor-pointer"
        >
          <option value="" class="bg-white text-black">
            NGN - Nigeria Naira
          </option>
          <option value="" class="bg-white text-black">
            USD - American Dollar
          </option>
          <option value="" class="bg-white text-black">
            GBP - British Pound
          </option>
        </select>
      </div>
    </div>
    <div>
      <div>
        <div class="flex items-center gap-2 bg-white border border-gray-200 rounded-full p-1">
            <span class="bg-[#003854] text-white text-sm rounded-full px-4 py-2">Monthly</span>
            <span class="pr-4"> Annual (save 2 months)</span>
        </div>
        <div class="flex items-center gap-2">
            <PricingCard v-for="price in pricing" :key="price.id" :pricing="price" />
        </div>
      </div>
    </div>
  </div>
</template>
