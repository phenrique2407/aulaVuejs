<script setup>
import { ref } from 'vue'
import CustomButton from '../components/CustomButton.vue'

const cliques = ref(0)
</script>

<template>
  <section class="card">
    <h2>1. Arquitetura baseada em componentes (SFC)</h2>
    <p>HTML, CSS e JavaScript juntos em um único arquivo .vue.</p>
    <!-- props: rotulo | evento: clicado -->
    <CustomButton rotulo="Clique aqui" @clicado="cliques++" />
    <p>O componente filho emitiu o evento {{ cliques }} vez(es).</p>
  </section>
</template>
