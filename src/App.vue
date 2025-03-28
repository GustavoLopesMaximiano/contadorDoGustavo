<script setup>
import { ref } from 'vue'

const contador = ref(0)

function incrementar() {
  contador.value++
}

function decrementar() {
  if(contador.value !== 0) {
    contador.value--
  }
  
}

function resetar() {
  contador.value = 0;
}
</script>

<template>
    <h1>contador</h1>
    <p>Contador: {{ contador }}</p>
    <button @click="incrementar" class="botao1">+</button>
    <button @click="decrementar" class="botao1">-</button>
    <button @click="resetar" class="botao1">reset</button>
</template>

<style scoped>

</style>
