<script setup>
</script>

<template>
  <footer>
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
    Coded by <a href="#">Chuck Smith</a>.
  </footer>
</template>

<style lang="scss" scoped>
footer {
  grid-area: footer;
  font-size: 0.75rem;
  color: var(--color-black);

  a {
    color: var(--color-black);

    &:hover {
      color: red;
    }
  }
}
</style>