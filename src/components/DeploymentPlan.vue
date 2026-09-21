<script setup>
import Plans from '@/components/Plans.vue';
import plans from "@/plans.json"

</script>

<template>
    <div class="bg-gray-200 flex items-center justify-center text-center py-24">
        <div class="w-full max-w-7xl flex flex-col items-center justify-center gap-8">
            <h1 class="text-5xl font-bold tracking-tight">Deployment Plan</h1>
            <p class="max-w-md text-xs text-gray-500 font-light"> 
                Choose the deployment edition that best aligns with your organization's 
                requirements, resources, and strategic objectives.
            </p>
            <div class="flex flex-col lg:flex-col items-center gap-4">
                <Plans v-for="plan in plans.plans" :key="plan.id" :plans="plan" />
            </div>
        </div> 
    </div>
</template>