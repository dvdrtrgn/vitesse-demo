<script setup>
import { ref } from 'vue'
const myColor = ref('red')
</script>

<template>
  <button @click="myColor = myColor === 'red' ? 'green' : 'red'">
    ▶️[ My color is {{ myColor }} ]◀️
  </button>
</template>

<style>
  button {
    color: v-bind(myColor);
  }
</style>
