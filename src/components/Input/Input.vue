<script setup>
const { modelValue, placeholder, name } = defineProps({
  modelValue: String,
  placeholder: String,
  name: String,
});
const emit = defineEmits(["update:modelValue"]);

function handleInput(event) {
  emit("update:modelValue", event.target.value);
}
</script>

<template>
  <input
    :name="name"
    :placeholder="placeholder"
    :value="modelValue"
    class="input"
    @input="handleInput"
  />
</template>

<style scoped>
.input {
  background: var(--color-bg-card);
  color: var(--color-primary);
  border-radius: var(--radius-sm);
  padding: var(--spacing-sm) var(--spacing-md);
  font-size: var(--font-2xs);
  max-width: 100%;
}

.input::placeholder {
  color: var(--color-primary-placeholder);
}
</style>
