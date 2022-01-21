<template>
  <footer>
    <div class="container">Developed by <strong>Kariston Stefane</strong></div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  padding: 1.5rem 12.5vw;
  text-align: center;
  font-size: 0.75rem;

  strong {
    color: $color-primary;
    font-family: $font-title;
  }
}
</style>
