<script setup>

import { ref } from "vue"
const count = ref(0);

function minus(){
  count.value--;
}


function add(){
  count.value++;
}
</script>

<template>
  <div>
    <h4>
      The Current Count is:
    </h4>
    <h3>{{count}}</h3>
    <button @click="minus">-</button>
    <button @click="add">+</button>
  </div>
</template>

<style scoped>
body{
  background-color: aliceblue;
  height: 100vh;
  width: 99vw;
  display: flex;
  justify-content: center;
  align-items: center;
  }
  
  div{
    text-align: center;
  }
</style>