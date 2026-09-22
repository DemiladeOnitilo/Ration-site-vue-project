<script setup>
import Plans from "@/components/Plans.vue";
import plans from "@/plans.json";
</script>

<template>
  <div
    class="bg-gray-200 flex items-center justify-center px-6 py-16 lg:px-0 lg:py-24"
  >
    <div
      class="w-full max-w-7xl flex flex-col items-center justify-center gap-8"
    >
      <h1 class="text-4xl lg:text-5xl font-bold tracking-tight">
        Deployment Plan
      </h1>
      <p
        class="max-w-xl lg:max-w-md text-md lg:text-sm text-center text-gray-500 font-light"
      >
        Choose the deployment edition that best aligns with your organization's
        requirements, resources, and strategic objectives.
      </p>
      <div class="flex flex-col lg:flex-row items-center gap-4">
        <Plans v-for="plan in plans.plans" :key="plan.id" :plans="plan" />
      </div>
    </div>
  </div>
</template>
