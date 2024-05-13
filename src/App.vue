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
    <div class="info">
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
    width: fit-content;
  }

  .name, .info{
    width: 250px;
  }

  hr{
    margin: 1rem;
    height: 50%;
  }

  @media screen and (max-width: 768px){
    main{
      flex-direction: column;
      text-align: center;
    }

    hr{
      margin: 1.5rem 0 1.5rem 0;
      height: 2px;
      width: 100%;
      background-color: white;
      border: none;
    }

    .name, .info{
      width: 350px;
    }
  }
</style>