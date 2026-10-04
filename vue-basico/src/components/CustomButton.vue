<script setup>
defineProps({
  rotulo: String,
})

const emit = defineEmits(['clicado'])
</script>

<template>
  <button class="btn-custom" @click="emit('clicado')">
    {{ rotulo }}
  </button>
</template>

<style scoped>
.btn-custom {
  background-color: #42b883;
  color: white;
  padding: 8px 16px;
  border: 0;
  border-radius: 4px;
  cursor: pointer;
}
</style>
