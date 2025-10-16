<script setup></script>

<template>
  <button class="button"><slot></slot></button>
</template>

<style scoped>
.button {
  border-radius: var(--radius-sm);
  background: var(--color-button-gradient);
  padding: var(--spacing-sm);
  font-size: var(--font-2xs);
  font-weight: var(--font-weight-semibold);
  color: var(--color-primary);
  cursor: pointer;
}
.button:hover {
  background: var(--color-button-gradient-inverted);
}
</style>
