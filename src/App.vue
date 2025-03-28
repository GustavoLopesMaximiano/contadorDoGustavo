<script setup>
import { ref } from "vue";

const contador = ref(0)

function incrementar() {
  contador.value++
}

function decrementar() {
  contador.value--
}
</script>

<template>
  <h1>contador</h1>
  <p>Contador: {{ contador }}</p>
  <button @click="incrementar" class="botao1">+</button>
  <button @click="decrementar" class="botao1">-</button>
</template>

<style scoped>
  
</style>
