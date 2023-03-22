<script setup>
import { ref } from 'vue';
let count = ref(0)

const addTOCounter = () =>
{
  count.value = count.value + 1
}

const substractToCount = () =>
{
  count.value = count.value - 1
}

</script>

<template>
  <main>
    <div>
      <h3>Hello From Vue</h3>
      <h1>{{ count }}</h1>
      <button @click="substractToCount()">-</button>
      <button @click="addTOCounter()">+</button>
    </div>
  </main>
</template>

<style scoped>
  main {
    background-color: aliceblue;
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  div {
    text-align: center;
  }
</style>
