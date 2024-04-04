<script setup lang="ts">
  import Name from './components/Name.vue'
  import Info from './components/Info.vue'
  import { ref } from 'vue';

  const name = ref<string>('Leandro Rocha');
</script>

<template>
  <main>
    <div class="name">
      <Name :name="name"/>
    </div>
    <hr>
    <div>
      <Info/>
    </div>
  </main>
</template>

<style global>
/* Add global styles of the project*/

  body{
    background-color: black;
    color: white;
    font-family: monospace;
    margin: 0;
  }

  main{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto 0 auto;
    height: 100vh;
    width: 500px;
  }

  .name, .info{
    width: 250px;
  }

  hr{
    margin: 1rem;
    height: 50%;
  }
</style>