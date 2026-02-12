<template>
  <div class="container">
    <h1>This is a test</h1>
    <h2>{{ count }}</h2>
    <h2>{{ ArrayArray }}</h2>
    <h2>{{ durrr }}</h2>
    <img @click="increment" src="/chocolate-chip-cookie.png" alt="" />
    <img @click="lololo" src="/images.jpg" />
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
const ArrayArray = ref(['1'])
const durr = ref(0)
function lololo() {
  ArrayArray.push('2')
  for (let i = 0; i < 20; i++) {
    ArrayArray.value.push(i)
    durr.value++
    console.log('pushed')
  }
  for (array in ArrayArray) {
    ArrayArray.value.push('ice cream')
    console.log('pushed2')
  }
}
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
