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
        font-size: 4rem;
    }

    @media screen and (max-width: 768px){
        h1{
            text-align: center;
            margin: 0;
        }
    }
</style>