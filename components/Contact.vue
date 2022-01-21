<template>
  <section id="contact">
    <div class="container">
      <h2 class="title">Contact</h2>
      <p class="text">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ullam illum
        magni aperiam, cumque maiores alias est error iusto sint tenetur.
      </p>

      <div class="spacer"></div>

      <h3 class="subtitle">Let's talk</h3>

      <div class="grid">
        <a href="https://wa.me/5548984783746" class="button" target="_blank"
          ><i class="icon-whatsapp"></i>WhatsApp</a
        >
        <a href="mailto:hi@kariston.dev" class="button" target="_blank"
          ><i class="icon-envelope"></i>E-mail</a
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.text {
  line-height: 150%;
  margin: 0 0 1.5rem;
}

.grid {
  gap: 1rem;

  @media (min-width: 768px) {
    display: flex;
  }
  @media (min-width: 1200px) {
    justify-content: flex-start;
  }
}

.button {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  background-color: $color-primary;
  color: $color-bg-alt;
  border: none;
  border-radius: 0.25rem;
  padding: 1rem 1.5rem;
  font: 700 1rem $font-title;
  text-decoration: none;

  i {
    font-size: 1.25rem;
  }
}
</style>
