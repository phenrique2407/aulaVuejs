<script setup>
import { useCounterStore } from '../stores/counter'

const store = useCounterStore()
</script>

<template>
  <section class="card">
    <h2>4. Ecossistema: Vue Router + Pinia</h2>
    <p>Contador global: {{ store.count }}</p>
    <p>Dobro: {{ store.doubleCount }}</p>
    <button @click="store.increment">Incrementar na store</button>
    <p><small>Navegue entre as abas: o valor da store é mantido.</small></p>
  </section>
</template>
