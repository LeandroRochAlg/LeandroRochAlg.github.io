<script setup lang="ts">
// allow the component to receive a prop named `name`
defineProps<{ name: string }>()
</script>

<template>
    <h1>{{ name }}</h1>
</template>

<style scoped>
    h1{
        text-align: right;
    }
</style>