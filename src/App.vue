<script setup>
import Navbar from '@/components/Navbar.vue';
import Hero from '@/components/Hero.vue';
import MessagesSection from '@/components/MessagesSection.vue';
import WhyRation from '@/components/WhyRation.vue';
import PricingPlans from '@/components/PricingPlans.vue';
import DeploymentPlan from '@/components/DeploymentPlan.vue';
import FAQs from '@/components/FAQs.vue';
import CTA from '@/components/CTA.vue';
import Footer from '@/components/Footer.vue';
</script>

<template>
  <div class="w-screen h-screen"> 
    <Navbar />
    <Hero />
    <MessagesSection />
    <WhyRation />
    <PricingPlans />
    <DeploymentPlan />
    <!-- <FAQs /> -->
    <CTA />
    <Footer />
  </div>
</template>