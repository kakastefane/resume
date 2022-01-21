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

      <div class="spacer"></div>

      <h2 class="subtitle">Get in touch</h2>
      <ul class="social">
        <li class="social__item">
          <a
            href="https://github.com/kakastefane"
            title="GitHub"
            class="social__link"
            target="_blank"
            ><i class="icon-github"></i
          ></a>
        </li>
        <li class="social__item">
          <a
            href="https://linkedin.com/in/karistonstefane"
            title="Linkedin"
            class="social__link"
            target="_blank"
            ><i class="icon-linkedin"></i
          ></a>
        </li>
        <li class="social__item">
          <a
            href="https://instagram.com/kakastefane"
            title="Instagram"
            class="social__link"
            target="_blank"
            ><i class="icon-instagram"></i
          ></a>
        </li>
        <li class="social__item">
          <a
            href="https://twitter.com/kakastefane"
            title="Twitter"
            class="social__link"
            target="_blank"
            ><i class="icon-twitter"></i
          ></a>
        </li>
      </ul>
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

  @media (min-width: 768px) {
    font-size: 1.25rem;

    strong {
      font-size: 3rem;
    }
  }

  @media (min-width: 1024px) {
    strong {
      font-size: 3.5rem;
    }
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

.social {
  display: flex;
  list-style: none;
  gap: 1rem;

  &__item {
    display: flex;
  }

  &__link {
    text-decoration: none;
    color: $color-text;
    font-size: 1.5rem;

    &:hover {
      color: $color-primary;
    }
  }
}
</style>
