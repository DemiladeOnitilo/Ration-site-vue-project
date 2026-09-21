<script setup>
import Logo from "@/components/Logo.vue";
</script>

<template>
  <nav class="absolute right-0 left-0 top-0 w-full flex justify-center items-center px-20 pt-6 lg:pt-16 z-999">
    <div class="w-full max-w-7xl flex justify-between items-center">
      <div>
        <Logo />
      </div>

      <div class="flex items-center gap-4 lg:gap-12 text-white text-xs lg:text-md">
        <p class="cursor-pointer group relative pb-1">
          Home
          <span
            class="absolute left-0 -bottom-1 w-full h-[2px] bg-white scale-x-0 origin-center transition-transform duration-300 group-hover:scale-x-100"
          ></span>
        </p>
        <p class="cursor-pointer group relative pb-1">
          Features
          <span
            class="absolute left-0 -bottom-1 w-full h-[2px] bg-white scale-x-0 origin-center transition-transform duration-300 group-hover:scale-x-100"
          ></span>
        </p>
        <p class="cursor-pointer group relative pb-1">
          Pricing
          <span
            class="absolute left-0 -bottom-1 w-full h-[2px] bg-white scale-x-0 origin-center transition-transform duration-300 group-hover:scale-x-100"
          ></span>
        </p>
        <p class="cursor-pointer group relative pb-1">
          Docs
          <span
            class="absolute left-0 -bottom-1 w-full h-[2px] bg-white scale-x-0 origin-center transition-transform duration-300 group-hover:scale-x-100"
          ></span>
        </p>
        <p class="cursor-pointer group relative pb-1">
          Contacts
          <span
            class="absolute left-0 -bottom-1 w-full h-[2px] bg-white scale-x-0 origin-center transition-transform duration-300 group-hover:scale-x-100"
          ></span>
        </p>
      </div>

      <div>
        <button
          class="bg-[#069] hover:bg-cyan-600 text-white text-xs lg:text-sm font-medium px-6 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer"
        >
          Get Started
        </button>
      </div>
    </div>
</nav>
</template>
