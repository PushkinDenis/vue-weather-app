<script setup>
import Button from "./components/Button/Button.vue";
</script>

<template>
  <main class="main"><Button>Сохранить</Button></main>
</template>

<style scoped>
.main {
  display: flex;
  background: var(--color-bg-main);
  padding: var(--spacing-3xl) var(--spacing-2xl);
  border-radius: var(--radius-md);
}
</style>
