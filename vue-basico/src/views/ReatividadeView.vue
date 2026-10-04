<script setup>
import { ref, reactive } from 'vue'

// Estado reativo simples com ref
const contador = ref(0)

// Estado reativo de objeto com reactive
const usuario = reactive({
  nome: 'Alice',
  idade: 25,
})

function incrementar() {
  contador.value++ // ref precisa do .value no script
  usuario.idade++  // reactive altera as propriedades diretamente
}
</script>

<template>
  <section class="card">
    <h2>3. Sistema de reatividade</h2>
    <p>Contador: {{ contador }}</p>
    <p>Usuário: {{ usuario.nome }} ({{ usuario.idade }} anos)</p>
    <button @click="incrementar">Incrementar idade e contador</button>
  </section>
</template>
