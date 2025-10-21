<script setup>
import { ref } from "vue";
import Button from "./components/Button/Button.vue";
import Input from "./components/Input/Input.vue";

const username = ref("");
const password = ref("");
</script>

<template>
  <main class="main">
    <Button>Сохранить</Button>
    <Input v-model="username" placeholder="Введите город" name="input" />
    <Input v-model="password" placeholder="Пароль" name="password" />
    <p>Ваш город:{{ username }}</p>
    <p>Ваш парол:{{ password }}</p>
  </main>
</template>

<style scoped>
.main {
  display: flex;
  background: var(--color-bg-main);
  padding: var(--spacing-3xl) var(--spacing-2xl);
  border-radius: var(--radius-md);
}
</style>
