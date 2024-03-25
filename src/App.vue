<script setup>
import { ref } from 'vue'

const titulo = ref('Título')
</script>

<template>
  <h1>{{ titulo }}</h1>
  <div class="container">
    <div class="formulario">
      <h2>Formulário</h2>
      <input type="text" v-model="titulo"/>
    </div>
    <div class="resultado">
      <h2>Resultado</h2>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  column-gap: 1.5rem;
  width: 100vw;
}

.formulario,
.resultado {
  width: 45%;
  border-radius: 10px;
  padding: 10px;
}

.resultado {
  background-color: #c4c4c4;
}
.formulario {
  background-color: #c4c500;
}
</style>
