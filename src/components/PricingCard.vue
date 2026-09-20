<script setup>
    import { defineProps } from 'vue';

    const props = defineProps({
        price: Object
    })
</script>

<template>
    <div class="bg-white flex flex-col gap-6 rounded shadow-xl">
        <div>
            <p>{{ price.type }}</p>
            <h3>{{ price.title }}</h3>
            <h2>{{ price.amount }}</h2>
        </div>
    </div>
</template>