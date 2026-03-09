<script setup>
    import { ref } from 'vue';

    const props = defineProps({
        name: String
    });
</script>

<template>
    <h2>Hello, {{ name }}!</h2>
</template>