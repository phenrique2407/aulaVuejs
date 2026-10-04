<script setup>
import { ref } from 'vue'

const exibeLista = ref(true)
const linguagens = ref(['JavaScript', 'TypeScript', 'Vue.js'])

function alternarExibicao() {
  exibeLista.value = !exibeLista.value
}
</script>

<template>
  <section class="card">
    <h2>2. Renderização declarativa e diretivas</h2>
    <button @click="alternarExibicao">
      {{ exibeLista ? 'Ocultar' : 'Mostrar' }} Lista
    </button>

    <ul v-if="exibeLista">
      <li v-for="item in linguagens" :key="item">
        {{ item }}
      </li>
    </ul>
  </section>
</template>
