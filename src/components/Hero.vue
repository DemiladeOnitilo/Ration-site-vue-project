<script setup>
import heroImg from "@/assets/images/hero-img.png";
import clientLogoOne from "@/assets/images/client-one.png";
import clientLogoTwo from "@/assets/images/client-two.png";
import { Comments } from "@primeicons/vue";
</script>

<template>
  <div
    class="min-h-screen relative bg-[#003854] flex flex-col items-center justify-center gap-6 lg:gap-12 pt-40 lg:pt-52 overflow-hidden"
  >
    <div
      class="absolute top-[-40px] lg:top-[-190px] border-1 border-white/10 border-dashed rounded-full p-90 lg:p-180"
    ></div>
    <div
      class="absolute top-[40px] lg:top-[-30px] border-1 border-white/10 border-dashed rounded-full p-60 lg:p-120"
    ></div>
    <div
      class="absolute top-[160px] lg:top-[190px] border-1 border-white/10 border-dashed rounded-full p-30 lg:p-60"
    ></div>

    <div
      class="flex flex-col items-center justify-center gap-6 text-center max-w-xl lg:max-w-2xl z-10 px-6 lg:px-0"
    >
      <h1
        class="text-3xl md:text-4xl lg:text-5xl lg:text-6xl text-white font-bold tracking-tight"
      >
        Communicate and Collaborate
        <span class="text-cyan-600">Seamlessly.</span>
      </h1>
      <p class="text-white text-sm md:text-md lg:text-lg">
        Ration is a messaging and collaboration platform that offers intuitive,
        flexible and extensible features
      </p>
    </div>

    <div class="flex items-center gap-6 z-10">
      <button
        class="bg-[#069] hover:bg-cyan-600 text-white text-sm font-medium px-6 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer"
      >
        Request Demo
      </button>
      <button
        class="hover:bg-white/10 text-white text-sm font-medium border border-white/70 px-6 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer"
      >
        Learn More
      </button>
    </div>

    <div
      class="w-full max-w-[340px] md:max-w-2xl lg:max-w-5xl pt-16 lg:pt-4 -mb-30 md:-mb-70 lg:-mb-90 z-10 shadow-lg"
    >
      <img :src="heroImg" alt="Hero Image" class="w-full" />
    </div>

    <div
      class="relative w-full bg-white flex flex-col justify-center items-center gap-2 pt-30 md:pt-70 lg:pt-90 pb-14"
    >
      <h2 class="text-md md:text-xl lg:text-2xl tracking-tight">
        Our Trusted Clients
      </h2>
      <div class="flex items-center gap-6">
        <img :src="clientLogoOne" alt="Client Logo One" class="w-12 lg:w-18" />
        <img :src="clientLogoTwo" alt="Client Logo Two" class="w-12 lg:w-18" />
      </div>
      <div
        class="absolute hidden lg:block bottom-14 right-20 bg-[#069] text-white rounded-full p-2 lg:p-4 hover:bg-cyan-600 hover:scale-[1.05] transition-all duration-300 ease-in-out cursor-pointer"
      >
        <Comments :size="30" />
      </div>
    </div>
  </div>
</template>
