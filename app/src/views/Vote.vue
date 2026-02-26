<template>
  <div class="container">
    <h1>Sordland 1954 Constitution</h1>
    <h3>
      USP (Conservative) Approval:
      <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <h3>
      USP (Reformist) Approval: <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <h3>
      NFP (Ethno-Nationalist) Approval: <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <h3>
      PFJP (Western Liberalism) Approval: <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <h3>
      WPB (Minority Rights) Approval: <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <img @click="increment" src="" alt="" />
    <img @click="preview" src="" />
    <button>reset</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const USP_Liberal_love = ref(50)
const USP_Conservative_love = ref(50)
const NFP_love = ref(50)
const PFJP_love = ref(50)
const WPB_love = ref(50)
const Current_arrow = ref(1)
function increment() {
  count.value -= 5
}
const SnowArray = ref(['1'])
console.log(SnowArray)
function preview() {}
</script>

<style scoped>
img {
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 40vh;
  max-width: 20vw;
}
</style>
