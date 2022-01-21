<template>
  <footer>
    <div class="container">
      Designed and developed by <strong>Kariston Stefane</strong><br />Built
      with <strong>NuxtJS</strong>
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.container {
  padding: 1.5rem 12.5vw;
  text-align: center;
  font-size: 0.75rem;
  background-color: $color-bg-alt;
  line-height: 150%;

  strong {
    color: $color-primary;
    font-family: $font-title;
  }
}
</style>
