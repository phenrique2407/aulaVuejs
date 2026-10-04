<script setup>
// Vue Router: <RouterLink> e <RouterView> fazem a navegação no lado do cliente
</script>

<template>
  <main>
    <h1>Vue.js: conceitos básicos</h1>
    <nav class="menu">
      <RouterLink to="/">1. SFC</RouterLink>
      <RouterLink to="/diretivas">2. Diretivas</RouterLink>
      <RouterLink to="/reatividade">3. Reatividade</RouterLink>
      <RouterLink to="/store">4. Pinia</RouterLink>
    </nav>
    <RouterView />
  </main>
</template>

<style scoped>
.menu { display: flex; flex-wrap: wrap; gap: 8px; margin: 12px 0; }
.menu a { color: var(--texto); text-decoration: none; padding: 6px 12px; border-radius: 4px; background: var(--card); }
.menu a.router-link-exact-active { background: var(--verde); color: #fff; }
</style>
