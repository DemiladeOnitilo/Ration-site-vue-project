<script setup>
import { shallowRef } from "vue";
import WhyRationCard from "@/components/WhyRationCard.vue";
import { CreditCard, FaceSmile, Headphones, Server } from "@primeicons/vue";

const cardItems = shallowRef([
  {
    id: 1,
    img: FaceSmile,
    title: "Friendly UI",
    description:
      "Designed with simplicity in mind from ground-up for easy adoption.",
  },
  {
    id: 2,
    img: Server,
    title: "Scalable Platform",
    description:
      "Expand your infrastructure to cater for a growing number of users.",
  },
  {
    id: 3,
    img: CreditCard,
    title: "Flexible Pricing",
    description: "Choose from a variety of pricing plans that fit your budget.",
  },
  {
    id: 4,
    img: Headphones,
    title: "24/7 Support",
    description: "Dedicated support team available around the clock to assist",
  },
]);
</script>

<template>
  <div
    class="bg-white flex flex-col lg:flex-row lg:justify-center gap-4 px-6 py-16 lg:px-0 lg:py-24"
  >
    <div class="w-full w-full lg:max-w-md flex flex-col gap-4 lg:gap-6 px-2">
      <div class="w-full flex flex-col gap-1">
        <p class="text-2xl lg:text-sm text-[#069] font-medium">
          Why Choose Ration
        </p>
        <h2 class="text-4xl md:text-5xl lg:text-4xl font-bold tracking-tight">
          Easily extendible. <br />
          Thoughtful UI/UX. <br />
          Flexible Pricing.
        </h2>
      </div>
      <p class="text-xl lg:text-sm">
        Smart APIs, seamless experiences, and open-source value, keeping
        innovation simple and costs low.
      </p>
      <button
        class="w-full md:w-fit bg-[#069] hover:bg-cyan-600 text-white text-sm font-medium px-10 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer"
      >
        Get Started
      </button>
    </div>
    <div class="grid md:grid-cols-2 gap-4">
      <WhyRationCard
        v-for="item in cardItems"
        :key="item.id"
        :cardItems="item"
      />
    </div>
  </div>
</template>
