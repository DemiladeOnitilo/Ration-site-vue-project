<script setup>
import Navbar from '@/components/Navbar.vue';
import Hero from './components/Hero.vue';
import MessagesSection from './components/MessagesSection.vue';
import WhyRation from './components/WhyRation.vue';
import PricingPlans from './components/PricingPlans.vue';
</script>

<template>
  <div class="w-full h-screen"> 
    <Navbar />
    <Hero />
    <MessagesSection />
    <WhyRation />
    <PricingPlans />
  </div>
</template>