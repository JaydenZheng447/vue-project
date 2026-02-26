<template>
  <div class="container">
    <h1>Sordland 1954 Constitution</h1>
    <h3>
      USP (Conservative) Approval:
      <span>{{ USP_Conservative_love }}%</span>
    </h3>
    <h3>
      USP (Reformist) Approval: <span>{{ USP_Liberal_love }}%</span>
    </h3>
    <h3>
      NFP (Ethno-Nationalist) Approval: <span>{{ NFP_love }}%</span>
    </h3>
    <h3>
      PFJP (Western Liberalism) Approval: <span>{{ PFJP_love }}%</span>
    </h3>
    <h3>
      WPB (Minority Rights) Approval: <span>{{ WPB_love }}%</span>
    </h3>
    <img @click="increment" src="" alt="" />
    <img @click="preview" src="" />
    <h2>Amendment 1: The Supreme Court</h2>
    <p>The</p>
    <h2>Section 1: Term Limits</h2>
    <p></p>
    <h2>Section 1: Term Limits</h2>
    <p></p>
    <h2>Section 1: Term Limits</h2>
    <p></p>
    <button>&#8592</button>
    <button>&#8594</button>
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
const s2a = "No term limits"
const s2b = "Two-term limit"

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
