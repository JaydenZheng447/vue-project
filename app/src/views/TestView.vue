<template>
  <div class="container">
    <h1>This is a test</h1>
    <h2>{{ count }}</h2>
    <h2>{{ ArrayArray }}</h2>
    <img @click="increment" src="/chocolate-chip-cookie.png" alt="" />
    <div @click="lololo">Hey check me out</div>
    <button>reset</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const count = ref(0)
function increment() {
  count.value++
}
function lololo() {
  for (let i = 0; i < 20; i++) {
    ArrayArray.push(i)
  }
  for (array in ArrayArray) {
    ArrayArray.push('ice cream')
  }
}
const ArrayArray = ref(['test array'])
</script>

<style scoped>
img {
  width: 200px;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 40vh;
}
</style>
