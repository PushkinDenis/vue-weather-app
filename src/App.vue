<script setup></script>

<template>
  <header>Header</header>
  <main>
    <button>Кнопка</button>
    <div class="div1">Надпись</div>
    <div class="div2">Надпись</div>
    <div class="div3">Надпись</div>
    <div class="div4">Надпись</div>
  </main>
  <footer>Footer</footer>
</template>

<style scoped>
main {
  display: flex;
  min-width: 100%;
  height: 100vh;
  background: var(--color-background);
  align-items: center;
  justify-content: center;
}
button {
  padding: 0 4rem 0 4rem;
  height: 4rem;
  background: var(--color-button-gradient);
  color: var(--color-white);
  border-radius: var(--radius-large);
  font-size: 16px;
}
.div2 {
  font-weight: var(--font-weight-medium);
  color: var(--color-white);
}
.div3 {
  font-weight: var(--font-weight-semibold);
  color: var(--color-white);
}
.div4 {
  font-weight: var(--font-weight-bold);
  color: var(--color-white);
}
</style>
