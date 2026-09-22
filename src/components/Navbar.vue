<script setup>
import Logo from "@/components/Logo.vue";
import { ref } from "vue";

const navItems = ref(["Home", "Features", "Pricing", "Docs", "Contacts"]);
</script>

<template>
  <nav
    class="absolute inset-x-0 top-0 flex justify-center items-center px-2 lg:px-20 pt-10 lg:pt-12 z-999"
  >
    <div class="w-full max-w-7xl flex justify-between items-center">
      <div>
        <Logo />
      </div>

      <div
        class="hidden md:flex items-center gap-4 lg:gap-12 text-white text-sm lg:text-md"
      >
        <p
          v-for="item in navItems"
          :key="item"
          class="group cursor-pointer relative pb-1"
        >
          {{ item }}
          <span
            :class="[
              item === 'Home'
                ? 'scale-x-100'
                : 'scale-x-0 group-hover:scale-x-100',
              'absolute left-0 -bottom-1 w-full h-[2px] bg-white  origin-center transition-transform duration-300 ',
            ]"
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
