<template>
  <section id="home">
    <div class="container">
      <h1 class="iam">Hello, I'am <strong>Kariston Stefane</strong></h1>
      <p class="about">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia dolore
        consectetur molestiae obcaecati ad harum totam rem magnam, numquam
        nobis, sapiente voluptates aspernatur reiciendis dignissimos
        voluptatibus, id repudiandae alias laborum.
      </p>
      <button class="button">Download CV</button>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#home {
  min-height: 100vh;
  background-color: $color-bg-alt;
}

.iam {
  display: flex;
  flex-direction: column;
  font-weight: 400;
  gap: 1rem;

  font-size: 1rem;
  margin: 0 0 1.5rem;

  strong {
    font-size: 2.5rem;
    font-family: $font-title;
    font-weight: 700;
    line-height: 100%;
    color: $color-primary;
  }
}

.about {
  margin: 0 0 2rem;
  line-height: 150%;
}

.button {
  background-color: $color-primary;
  color: $color-bg-alt;
  border: none;
  border-radius: 0.25rem;
  padding: 1rem 1.5rem;
  font: 700 1rem $font-title;
}
</style>
